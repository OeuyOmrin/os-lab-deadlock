Level 3 – Local Circular Wait

Both sync_up and sync_down hold one vault lock and wait for the other, creating a circular wait. The scripts freeze because all four deadlock conditions are met locally.

Level 4 – Site-to-Site Sync

Player A and Player B each hold their local vault lock and wait for the other’s lock. This distributed circular wait freezes both users, simulating a distributed denial-of-service.

Level 5 – Global Resource Ordering

All scripts acquire locks in the same global order (Alpha → Beta). Circular wait is broken, so simultaneous scripts run sequentially without deadlock.

Level 6 – Deadlock Recovery (Timeout)

Scripts use a timeout when waiting for a lock. If the lock is unavailable, the script aborts gracefully, preventing infinite waits and keeping the system responsive.

Level 7 – Safe Ejection (Teardown)

Loop devices are unmounted and detached safely, and symlinks removed. This prevents file system corruption and orphaned devices, ensuring system stability.
