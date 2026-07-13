**Introduction of the project:**

Encryption is a process in which when sending data as plaintext (raw readable message), gets scrambled and turned into an unreadable message send across a communications channel, it is scrambled via an algorithm and a key. The key idea about encryption is that even if a message is intercepted by a third party during the transmission process it cannot be understood or decrypted without the use of the key.
My project is focused on making an encryption software where I develop my own version of an encryption technique and implement it so I can add a chat feature to a software to allow for at least 2 users to send end to end encrypted messages to each other and can be decoded at the other end. To achieve this I have researched different encryption methods and will use them to make a custom encryption algorithm that I can complete within the timeframe of the NEA

**Key ideas and research notes that go into thinking about the project:**
Common encryption used in messaging apps
The cipher WhatsApp uses is called the AES-256 cipher also known as The Core Block Cipher.
WhatsApp uses a combination of asymmetric and symmetric encryption to make up its end to end encryption, using a public key (only the recipient’s private key can unlock the public key).  The main cryptography process is called Extended Triple DIffle-Hellman form a stable chat session.
The symmetric part of WhatsApp’s encryption is using a single shared key to both encrypt and decrypt the information
The Asymmetric part is the use of two different keys a public key and a private key, the public key is used to lock/hide the message you’re sending and the private key is its pair and is used to unlock the message.
In order to be as secure as possible, WhatsApp uses a new unique and temporarily asymmetric key for every message to stop people intercepting the message and decrypting it because of the multiple use of the key. Even using a key twice can leave it vulnerable to being cracked.
A combination of both asymmetric and symmetric is used because the asymmetric establishes the secure session for users to chat on by combining public and private keys and symmetric is used for the actual messaging on the platform.

(Information Security Stack Exchange) 
(WhatsApp)

Telegram The cipher telegram uses is also AES-256 but they also created their own custom architecture called MTProto, the AES-256 is also paired with an operation called IGE which is essentially a failsafe that if an attacker gets a hold of a bit of data in transmission the rest of the message jumbles up and becomes an unreadable 	mess for everyone
	
Telegram uses Cloud Chats which involve using a client server encryption and the message is decrypted on the server side, this offers a less secure approach to encryption as it doesn’t promise end to end encryption like WhatsApp or other media apps promise. The cloud chats allow for multi device syncing and backups meaning these chats can potentially be stored and re accessed on a cloud server more easily accessible and prone to attacks.

Telegram also offers a service called Secret chats which is their end to end encrypted chat 

(Telegram Privacy Explained) ~ Unknown Author
(Telegram)  ~ End-to-End Encryption, Secret Chats

 

**The Cipher/Encryption I plan on making:**

AES-256 cipher is a complex encryption cipher using a block cipher that uses a 256 bits to make a key and 128 bits blocks with 14 rounds, it includes substitution, row shifting column mixing, round key addition.
The cipher I will be using will be a custom made simplified cipher inspired by the AES-256 cipher that is similarly used by WhatsApp and telegram, it is the go to cipher for encryption of text from one place to another.  I will make a similar structure inspired by the AES-256 but I will use 64 bits for the block size, 64 bits for the key 5 rounds and a block chain cipher.
	
Can I make the project technical enough to get maximum marks out of a project 	or am I limiting myself:
	Creating a custom encryption algorithm with rounds, blocks, IV generation, key uses
	Advanced OOP structure: Inheritance(see uml), Polymorphism: swapping encryption at runtime, different clients. Encapsulation: Hiding keys, Composition: MessageHandler, 	Abstraction: EncryptionAlgorithm, Recursion: Round function



**Research behind why do the project in the first place**
	What makes the project good:
An encryption chat software is a good NEA project because it allows a range of complex algorithmic skills and features that flow naturally into the project instead of being forcefully added. This project has real world relevance and allows for exploration into topics that are relevant to the course but beyond the specification. An encryption chat software allows for new skills to learn that won’t come up in education but also expands on the coding skills I already have but taking them to an upgraded level. 

**Is this doable in the time frame:**
As an NEA project worth 20% of the A level putting in enough detail and complexity within the given time frame is difficult and if not arranged carefully this project could become far more complex than I have time for, in order to keep on track after a substantial amount of time has passed I will compare my progress to my aims and objectives and make a decision on how much I can complete before the deadline.

**Existing Solutions:**
Surveys
Equations

**Key Algorithms:**
	
Software skills
How technical is this project and can it give the most amount of marks and not cap myself
Key algorithmic skills involved
Databases
OOP
Band A skills
Website Portability
“My NEA is going to be awesome

**Objectives/ Success Criteria**
Messages are encrypted from one end to the other
Messages are sent and received with a very small time delay < 50ms per message
Message is correctly decrypted to the original plaintext with no corruption or changes from the original
Each message uses its own symmetric key, so one key is not re used to maximise security
Messages are tracked and composed of their metadata that can be viewed
Any corrupted or invalid messages are dealt with and don’t crash the system
If someone tries to intercept the message, there is a failsafe protocol that alerts the system 
Messages can be started encrypted or they can start as plaintext
Messages are sent and received with a delay of < 200ms

Third  Party Client (Interview)
Archie Hollins (Student at Hills Road Sixth Form College)
Questions asked:

**Feedback:**

**Prototype**


**Modelling: UML Diagram **

 



(Smalley)“This is my test reference” (Coleman, Noah Colemans NEA reference test)
(Hills Road Sixth Form College) NEA Overview

