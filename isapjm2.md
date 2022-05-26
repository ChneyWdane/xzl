> 加密是通过在流模式下使用键控海绵结构来执行的，显著的区别是，首先调用IsapRk来生成子键K~E~^∗^．IsapEnc得到一个K
> -bit密钥K，一个K -bit nonce
> N和一个任意大的消息M作为输入，生成一个大小为\|M\|的密文C。该函数在算法3和图2.1d中描述。它首先使用标志f
> = ENC调用IsapRk进行加密，以选择初始值IV~KE~和z = n -
> k，从而派生出一个(n -
> k)位的子密钥K~E~^∗^．一旦这个子键生成，使用置换p~E~的常规基于海绵的流模式将在高速率r~H~下进行评估。IsapEnc是流模式，解密与M、C交换的角色相同。
>
> ![](media/image1.jpeg){width="2.388888888888889in"
> height="1.4444444444444444in"}![](media/image8.jpeg){width="2.388888888888889in"
> height="1.4444444444444444in"}
>
> (a)加密E(K, N, a, M） (b)解密D(K, N, A, C, T)
>
> ![](media/image16.jpeg){width="2.6527777777777777in"
> height="1.3888888888888888in"}
>
> ![FORMULA](media/image22.jpeg){width="4.694444444444445in"
> height="0.18055555555555555in"}
>
> ![](media/image23.jpeg){width="2.8194444444444446in"
> height="1.5944444444444446in"}
>
> \(d) IsapEnc
>
> ![](media/image34.jpeg){width="5.527777777777778in" height="1.375in"}
>
> \(e) IsapMac

图2.1。: Isap的加密算法E(K, N, A, M)和解密算法D(K, N, A, C,
T)组成IsapEnc流加密，IsapMac MAC和IsapRk rekeyying。
