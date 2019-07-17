# Legend

| Symbol | Description |
| :---: | :--- |
| **$msg$** | a message transmitted by a participating node to its peers during a specific step |
| **$sig\(x\)$** | the EdDSA signature of $x$ |
| **$H\(x\)$** | the SHA-256 hash of $x$ |
| **$r$** | the current round of the algorithm, which is equivalent to the number of blocks in the database plus one. $r &gt;= 1$ |
| **$s$** | the current step number of the algorithm in the round. $s &gt;= 1$ |
| **$B\_{r}$** | a block created in round $r$, which equals to { **$r$**, **$ID\_{producer}$**, **$Q\_{r}$**, **$H\(B\_{r}\)$**, **$H\(B\_{r-1}\)$**, **$sig\(B\)$**, **$PAY\_{r}$**, **$CERT\_{Br}$** } |
| **$H\(B\_{r}\)$** | the SHA-256 hash of **$B\_{r}$** |
| **$PAY\_{r}$** | the set of transactions contained in block **$B\_{r}$** |
| **$Q\_{r}$** | the shared randomness seed of round **$r$** |
| **$sig\(Q\_{r}\)$** | the signature of a random vector of the **$r$** round |
| **$sig\(B\_{r}\)$** | the signature of a block of the **$r$** round |
| **$l\(r\)$** | the round **$r$** leader - determines **$PAY\_{r}$**, creates **$B\_{r}$** and determines **$Q\_{r}$** |
| **$CERT\_{r}$** | a **$B\_{r}$** block certificate formed out of a set of `bba_signature` messages |
| **$VRF\(r, s\)$** | the ordered set of participants who act in step **$s$** of round **$r$** |
| **$VRFN\(r, s\)$** | the ordered set of indexes of **$VRF\(r, s\)$** participants who are registered on the current node and participate in step **$s$** of round **$r$** |
| **$id$** | an account identifier in the blockchain |
| **$A\_s$** | an array of account identifiers selected as participants in the step **$s$** |
| **$N\_s$** | an array of $A\_s$ indexes which correspond to the identifiers of users authorized on the current node in the step **$s$** |
| **$l$** | the id of the producer who is the leader in this round |
| **$ctx$** | the context of the current round as an object which contains all received messages for the round |
|  |  |
|  |  |
|  |  |

