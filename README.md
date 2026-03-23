Level3
A deadlock occurred because both scripts acquired the first lock and then w>

sync_up held Vault Alpha and was waiting for Vault Beta.
sync_down held Vault Beta and was waiting for Vault Alpha.
This satisfies the Circular Wait condition: a cycle of processes waiting fo>

Level 4.
A distributed deadlock occurred because each user locked their local vault >

Level 5.
By modifying Player B’s script to acquire Alpha first and Beta second, all >

Level 6.
The timeout strategy allows a script to wait for a resource for a limited t>


Level 7.
Proper teardown is critical because leaving a loop device mounted while del>
