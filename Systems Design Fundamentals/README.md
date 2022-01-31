# [SystemsExpert](https://www.algoexpert.io/systems/product)
 
## Systems Design Fundamentals
> Where the Coding Interview serves primarily as an assessment of your problem-solving ability, the Systems Design interview is a test of your engineering knowledge veiled behind the facade of an open-ended design question.

### 1. Design Fundamentals - Introduction
>* Coding Interviews tests a Software Engineer's ability to solve a problem.
>* They focus **less** on theoritical knowledge and **more** on problem solving ability.
>* Overall, if a coding interview problem is given to someone who has no coding background, no computer science background, they would likely be able to tackle the problem at least a little bit.
>* They wouldn't be able to know that they have to use a certain data structure to solve a problem optimally. But they would be able to conceptually tackle the problem. 

>* With Systems Design interviews on the other hand, that would not be possible.
>* If someone with no software engineeering background is given a canonical Systems Design interview question like design Youtube, design a website where millions of people can upload video content and billions of people can view that content and comment on it, like it, that person would not be able to answer this question properly.
>* Because Systems Design interviews really do require a lot of **knowledge** about Systems, about how to build Robust, Functional, and Scalable Systems.
>* That's where Design Fundamentals come into play.
>* **Design Fundamentals** are the **foundational knowledge** that is needed for **Systems Design interviews** just as Data Structures are the foundational knowledge that is needed for Coding Interviews.
>* Design Fundamentals are absolutely necessary. Without them one cannot tackle a Systems Design interview question.

>* There are lot of Design Fundamentals to know such as System, Availability, Database, Load Balancer, Cache, HTTP etc.

---

### 2. What Are Design Fundamentals?
>* Building scalable, production-ready applications is both art and science. Science, in that it requires **knowledge of many topics** in computer engineering; art, in that it demands an **eye for making smart design choices and piecing together** the right technologies.
>* Master both disciplines and you, too, can become a **Systems Expert**.

#### How Systems Design interviews actually work?
>* Systems Design interview questions are very **intentionally vague**.
>* They can **often be stated in just a few words** like **design Uber** or **design Facebook Messenger**, **design Youtube**.
>* And it is the **responsibility of the interviewee** to be able to take a two-word sentence, like design Uber and **turn it into a 45-minute discussion**.
>* So naturally that's gonna involve asking your interviewer questions, prodding them about what type of system you're building, what kind of functionality the system is gonna have to support, what characteristics we're gonna value in the system.
>* This type of **investigation** in a Systems Design interview is gonna **require a lot of fundamental Systems Design knowledge**.

>* Now the second thing that's important to note about Systems Design interviews is that, unlike with coding interviews, where a solution to coding interview question is either objectively correct or incorrect.
>* With **Systems Design interview questions**, there's a **lot more subjectivity**.
>* A **proposed solution** to a Systems Design interview question **may very well not be objectively correct or objectively incorrect**.
>* There might be certain concepts in Systems Design that could be used objectively incorrectly, if misinformed or if one doesn't have appropriate knowledge.
>* But, if you have the appropriate knowledge, if you are well informed, if you are prepared, then a suggested solution to a Systems Design interview question is not gonna be objectively correct or incorrect.
>* It's gonna be **your job** to **very confidently justify your solution**.
>* It's gonna be **your job** to explain, to **rationalize** why you've made certain choices, why you've **designed** parts of your system in **one way instead of another**.
>* It's gonna be **your job** to **make your interviewer understand** 
why your proposed solution is reasonable, why it's sound, and why it might be the best one. Or perhaps why it might not be the best one, why it might be one of many potential solutions.
>* It's gonna be **your job** to **eliminate any doubts that your interviewer might have** in some of your design choices.
>* It's gonna be **your job** to **defend your position, or to adapt your position** if your interviewer challenges it.
>* This is gonna be nearly **impossible** to do **without** the **proper fundamental knowledge** about Systems Design.
>* That's why Design Fundamentals are so critical to Systems Design interviews.

#### Categories of Systems Design
>* Design Fundamentals come in a lot of different flavors.
>* More specifically, they can be bucketed in **4 broad categories**, categories that are equally important, categories that are very much intertwined, and categories that kind of build upon each other.

##### 1st Category
>* The 1st category of design fundamentals is the **underlying or the foundational knowledge**.
>* These are gonna be design fundamentals where, if you don't understand them, you will at best have severe gaps in knowledge that will undermine your positions or your ability to defend your positions in a Systems Design interview and that will, at worst, make you basically incapable of even beginning to tackle a Systems Design interview.

>* **For example**, you have to know what the client server model is, to be able to design any modern day system.
>* Things like network protocols. You have to have some understanding of how machines communicate and interact with one another in order to be able to properly design a complex system.

> So that is the 1st category of Design Fundamentals, foundational Systems Design knowledge.

##### 2nd Category
>* The 2nd category of design fundamentals is **key characteristics of systems**.
>* These are gonna be the thiings that a you might want a System to have.
>* These are gonna be the things that you might be trading off when making certain design decisions.

>* Design fundamentals like availability, wait and see, throughput, redundancy, consistency etc., are the key characteristics of systems that one has to know about.

##### 3rd Category
>* The 3rd category of design fundamentals is **actual components of a system**.
>* These are gonna be the slightly more tangible things that you can **either have in a system or implement in a system**.
>* Things like load balancers, proxies, caches, rate limiting, leader election etc., are really gonna be the bread and butter of a system that you are designing.
>* These are the **key components** that are gonna allow your system to have the **key characteristics** that we just mentioned above.

##### 4th Category
>* The 4th category of design fundamentals is **actual tech, real existing products or services** that you can actually use in a system either as actual components in a system, or to achieve a certain characteristic in a system.
>* These are gonna be real tools, things like Zookeeper, Redis, Amazon S3, Google Cloud Storage etc.
>* These existing real-life tools that you can actually use in a Systems Design interview to build up your system.

>* The 4th category of design fundamentals is the one that's **often overlooked**.
>* Also, this is **very important** one that can really **round you off and make you shine** in a Systems Design interview,

> ***This is what design fundamentals really are.***

> And **being very well versed** in these design fundamentals, is what's gonna **allow you to tackle** these very vague Systems Design interview questions, **to make sound reasonable** design choices, **to justify** them, and **to convince** your interviewer that you are a great systems designer.

> There are a lot of design fundamentals to know and these are complicated subjects.

---

### 3. Client-Server Model
> A client is a thing that talks to servers. A server is a thing that talks to clients.
> The client-server model is a thing made up of a bunch of clients and servers talking to one anotther.

#### 6 Key Terms

- ***Client***
> A machine or process that **requests data or service from a server**.

> Note that a single machine or piece of software can be both a client and a server at the same time. For instance, a single machine could act as a server for end users and as a client for a database.

- ***Server***
> A machine or a process that **provides data or service for a client**, usually by listening for incoming network calls.

> Note that a single machine or piece of software can be both a client and a server at the same time. For instance, a single machine could act as a server for end users and as a client for a database.

- ***Client-Server Model***
> A paradigm by which modern systems are designed, which consists of clients requesting data or service from servers and servers providing data or service to clients.

- ***IP Address***
> An address given to each machine connected to the public internet.
> IPv4 addresses consist of four members separated by dots: **a.b.c.d** where all four members are between 0 and 255. Special values include:
	>- **127.0.0.1**: Your own local machine. Also referred to as **localhost**.
	>- **192.168.x.y**: Your **private network**. For instance, your machine and all machines on your private wifi network will usually have the **192.168 prefix**.

- ***Port***
> In order for **multiple programs to listen** for new network connections on the **same machine without colliding**, they pick a port to listen on. A port is an integer between **0 and 65,535 (2<sup>16</sup> ports total)**.

> Typically, ports 0-1023 are reserved for system ports (also called well-known ports) and shouldn't be used by user-level processes. Certain ports have pre-defined uses, and although you usually won't be required to have them memorized, they can sometimes come in handy. Below are some examples:
	>- **22**: Secure Shell
	>- **53**: DNS lookup
	>- **80**: HTTP
	>- **443**: HTTPS

- ***DNS***
> Short for **Domain Name System**, it describes the entities and protocols involved in the translation from domain names to IP Addresses. Typically, machines make a DNS query to a well known entity which is responsible for returning the IP Address (or multiple ones) of the requested domain name in the response.

---

#### Understanding Client-Server Model
> This is an incredibly **important concept**.
> It's the **foundation of the modern internet**.
> The foundation of how computers speak to one another.
> And it's a very important thing to understand in the context of system design interviews.

> To understand Client-Server Model, let's explore/understand **what happens when we go to [algoexpert.io](algoexpert.io)**?

#### What happens when you open up your browser and type in your URL bar [www.algoexpert.io](www.algoexpert.io) and then press Enter? 
  >- Well, your browser, be it Google Chrome, or Safari, or Firefox, **your browser is a client**, and **AlgoExpert**, for the sake of this example, **is the server**.
  >- One important note to make here, is that the **client**, that is the browser, **doesn't know** actually what the server, or in this case, AlgoExpert is.
  >- All that it knows, is that it can communicate with it. It can speak to it, it can request stuff from it.
  >- But it doesn't actually know what the server represents.
  >- It will request information from the server, and then, based on that information, based on the response from the server, it'll be able to do stuff.

#### So, when you type [algoexpert.io](algoexpert.io) in your URL bar, at first your browser doesn't even know how to talk to AlgoExpert, or the server.
  >- What it does behind the scenes, actually, is it makes what's called a DNS query, to find out what the IP Address of [algoexpert.io](algoexpert.io) is, and only then it can really speak to AlgoExpert, the server.
  >- A **DNS Query** is a special request, that goes to a predetermined set of servers, and basically says "*Hey, what's the IP Address of [algoexpert.io](algoexpert.io)?*"
  >- An **IP Address** is just a **unique identifier** for a machine.
  >- All computers connected to the internet, have ways to find public IP Addresses, or at least, they have ways to discover routes to those addresses.
  >- And that means that, they can send data to IP Addresses.
  >- They can send packets of information, in the form of bytes, to IP Addresses.
  >- You can almost think of an IP Address as a mailbox, that some entity has granted to a machine.

  >- **For example**, in the case of AlgoExpert, it turns out that the entity that has granted AlgoExpert an IP Address is AlgoExpert's cloud provider, which happens to be Google Cloud Platform, in other words, Google.
  >- If you're on Unix operating system, for instance, a mac or a linux machine, open the terminal, type ```dig algoexpert.io```
  >- This command allows us to do DNS Queries and then displays the answer in the terminal.
  >- This **command gives the [algoexpert.io](algoexpert.io)'s IP Address**.
  >- And something very similar happens behind the scenes when in your browser, you type in [algoexpert.io](algoexpert.io).
  >- Your client, the browser, **makes a DNS Query**, **gets the IP Address back**, and then **knows how to communicate** directly with AlgoExpert.

#### So what happens next ?
  >- Your browser, let's say, Google Chrome, knows what [algoexpert.io](algoexpert.io) is because it has the IP Address.
  >- And it **sends an HTTP request** to this IP Address.
  >- HTTP is a **way to send information**, that server can understand.
  >- So, when we say that a browser, or a client, sends an HTTP request to the AlgoExpert servers, basically it sends a bunch of bytes, or characters, that are gonna get packed into what we call packets, in some special format, and that's gonna be sent over to the AlgoExpert servers.
  >- And that **request** is also gonna **contain** the **IP Address of the browser, or the computer**, and that's gonna be called as the **source of the request**. And that's gonna be really important because when the server gets that request, it's gonna know what IP Address it should send a response to.
  >- So the AlgoExpert server will use that source IP Address, which is contained in the HTTP request, and use it to send it's response, it'll know that it should send it's response to that source address.

#### There's one more thing that we need to talk about, which is ports.
  >- Servers are machines that are waiting to receive requests from other machines called clients.
  >- And once they get those requests, they can send responses to those clients.
  >- Now it turns out that a **server usually listens** for requests **on specific ports**.
  >- Any machine that has a distinct IP Address, has **16000 ports** that programs on the machine can listen to.
  >- And so when you are **communicating with another machine**, you actually have to **specify what port you wanna communicate on**.
  >- So as a client, when you are communicating with a server, you actually have to specify the port that you wanna communicate on.

> When we're talking about the Client-Server Model here, it turns out that **most clients actually know the port that they should use, depending on the protocol** that they are trying to speak to the server with.
  >- So for instance, if a client is trying to speak to a server, using the **HTTP** Protocol, it's always going to use **port 80**. This is just something that was decided on a long time ago, and that's just how it is.
  >If it's trying to speak to a server with **HTTPS**, it's gonna use **port 443**. Again, something that was decided on a long time ago.

#### So, when you type [algoexpert.io](algoexpert.io) in your browser, and everything that is mentioned above has happened, and eventually the AlgoExpert server receives the request, it's able to read the requests because it understands the HTTP format.
  >- And so the server understands that when you go to [algoexpert.io](algoexpert.io), you are **trying to see the HTML of AlgoExpert** and it returns in its response to the client.
  >- And the browser **receives the response** and then **renders the HTML** on the page.

> **This is incredibly important concept, because it's really through this Client-Server paradigm, that all computers talk to one another, all over the world.**
> **All the modern technologies that we see day to day are built on top of these concepts.**

---

### 4. Network Protocols
> IP packets. TCP headers. HTTP requests.

> As daunting as they may seem, these low-level networking concepts are essential to understanding how machines in a system communicate with one another. And as we all know, proper communication is key for thriving relationships! :smile:

#### 4 Key Terms

- ***IP***
> Stands for **Internet Protocol**. This network protocol outlines how almost all machine-to-machine communications should happen in the world. Other protocols like **TCP**, **UDP**, and **HTTP** are built on top of IP.

- ***TCP***
> Network protocol **built on top of the Internet Protocol (IP)**. Allows for **ordered, reliable data delivery** between machines over the public internet by creating a **connection**.

> TCP is usually **implemented in the kernel**, which exposes **sockets** to applications that they can use to stream data through an open connection.

- ***HTTP***
> The **H**yper**T**ext **T**ransfer **P**rotocol is a very common network protocol **implemented on top of TCP**. Clients make HTTP requests, and servers respond with a response.

##### Requests typically have the following schema:
>- host: string (exmaple: algoexpert.io)
>- port: integer (example: 80 or 443)
>- method: string (example: GET, PUT, POST, DELETE, OPTIONS or PATCH)
>- headers: pair list (example: "Content-Type" => "application/json")
>- body: opaque sequence of bytes

##### Responses typically have the following schema:
>- status code: integer (example: 200, 401)
>- headers: pair list (example: "Content-Length" => 1238)
>- body: opaque sequence of bytes

- ***IP Packet***
> Sometimes more broadly referred to as just a (network) **packet**, an IP packet is effectively the **smallest unit used to describe data** being sent over **IP**, aside from bytes. An IP packet consists of:
  >- an **IP header**, which contains the source and destination **IP addresses** as well as other information related to the network.
  >- a **payload**, which is just the data being sent over the network.

---

#### Understanding Network Protocols
> The topic of network protocols is one of those topics that tends to intimidate a lot of people. The words network and protocol put together just sound scary.
> The actual network protocols that exists out there are typically referred to by their acronyms like **IP**, **TCP**, **UDP**, and they naturally sound mysterious, foreign, and the majority of network protocols are admittedly very low level.
> They're things that most software engineers aren't gonna be dealing with on a day to day basis. And so all of these things put together make the topic of network protocols very intimidating.

> That being said, in the context of Systems Design interviews, network protocols actually aren't that intimidating.
> They are quite simple because you only need to know them at a high level.

#### What is a Protocol?
> A protocol is really just an **agreed upon set of rules for an interaction between two parties**.
> If two human beings cross each other on the streets and they vaguely know each other, they just exchange a few words, say hello to each other and all that.
> This is fairly common and this is effectively a commmunication protocol.

> In the context of networking, a protocol isn't going to be something for communication between two human beings but instead for **communication between two machines** (Clients/Servers).  
> Well these machines, clients and servers, interact with one another following network protocols.

#### What a Network Protocol consists of?
> A network protocol consists of the kinds of **messages** that are gonna be sent and received by machines, by clients and servers.
> The **format** of those messages, **how they are structured**, the **order** of those messages if they have an order, and whether or not they should be **some sort of response** to a message if there should be, what that **response should look like**, whether or not there should be **rules around when messages can be sent**, all of that stuff.

> There are a **lot of network protocols** out there.
> The majority of them you really don't need to know about at least in the context of Systems Design interviews and just general Software Engineering.
> There are few that are very popular and that are important to know about.
> We are gonna cover specifically **IP**, **TCP**, and **HTTP**.

- **IP**
	- IP stands for **Internet Protocol**.
	- IP is the acronym used in **IP** Address.
	- So an IP Address is literally an **Internet Protocol Address**.
	- There's a lot to know about Internet Protocol and the way it works.
	- The modern internet effectively runs on IP.
	- The modern internet effectively operates following the Internet Protocol.
	- And what that means is that, when a machine or a client for instance tries to interact with another machine or a server and it sends data to that other machine, that data is going to be sent in the form of what's known as an **IP Packet**.
	- IP Packet is the **fundamental unit of data** that is sent from one machine to another.
	- IP Packets are the **building blocks of communication between machines over the internet**.
	- Now, truthfully, there are other units beyond IP Packets because **IP Packets are actually made up of bytes**.
	- IP Packets have **2** main sections: ***IP Header*** and the ***Data***.
	- **IP Header** is the section of an IP Packet that is gonna be at the **beginning** of the packet.
	- Headers **contain all the information about the packet** and that is **stored in bytes**.
	- Namely, it contains the **source IP Address** of the packet. It contains **destination IP Address**.
	- If you have a single IP Packet, you know where that IP Packet is coming from and where it is going to.
	- **This is how information flows over the network, on the internet**.
	- This is how information knows to go from one machine to another.
	- Because all these IP Packets have the source and destination IP Addresses of the machines that they are coming from and going to.
	- The header also has other information like the **total size** of the packet, **version of the Internet Protocol** that this IP Packet is operating by.
	- There are **multiple versions of Internet Protocol** and today, there are really **2 versions in practice**.
	- There's **version 4 known as IPV4**, this is really what most of the modern day internet uses, and then there's **version 6, IPV6** which is now being used more and more.
	- **Based on the IP version**, the packet might look different. It might be structured a little differently, and a machine will know how it should interpret it based on that version.
	- The header is very small, anywhere between 20 and 60 bytes, and then the rest of the IP Packet is the data part of the IP Packet.
	- In the data portion of the IP Packet, the information that a machine is trying to send to another machine is gonna be stored.
	- Now IP Packets are limited in size. They are only **2 to the power of 16 bytes** which is only about **65,000 bytes**. This is only 0.065 mega bytes. That's really nothing.
	- If you are sending information over the network, you could imagine you might be sending an email, you might be sending a big file, you might be sending an image.
	- You are gonna be sending way more than 65,000 bytes.
	- In other words, if you are sending information over the network, that information, that data is likely not gonna fit in one IP Packet.
	- Now what happens is that, **it will fit into multiple IP Packets**,
	- This is where things get complicated. When you have multiple IP packets that are sent from one machine to another, if all you are using is the Internet Protocol, you don't actually have a way of guaranteeing that these packets are actually gonna be received. It's very possible that some of the packets are gonna get lost, over the network. And if that's the case, you won't have sent all of the data that you were trying to send.
	- You are also not guaranteeing the order in which the packets will be read or interpreted, and that's obviously not great because you want your packets to be ordered correctly such that your original data is sent in the correct order and in the correct structure that it's meant to be sent in.
>- **So Internet Protocol alone kind of falls apart here**.
>- **And this is where TCP comes into play**.

- **TCP**
	- TCP stands for **Transmission Control Protocol**.
	- TCP is **built on top of the Internet Protocol**.
	- It's really **meant to solve the issues that exists in the IP**.
	- It's meant to send IP Packets in an ordered way, meaning that you are guaranteeing the order in which the IP Packets will be read by the destination machine.
	- In a **reliable** way meaning that you are guaranteed to get those packets actually received by the destination machine or at the very least you will know if some packets keep failing from getting received and in an error-free way.
	- If some **IP Packets get corrupted for whatever reason** when they are being sent over the network, you will know and **you will be able to resend** those packets to make sure that they're received in an uncorrupted way.
	- This is what **TCP aims to solve** in a nutshell.
	- TCP is used in virtually all web applications and it allows you to send arbitarily long pieces of data to other machines because of those things that it solves that the Internet Protocol alone can't really accomplish.
	- An IP Packet has IP Header and the Data. **In TCP**, as TCP is built on top of IP, the IP Packet's data portion will have **TCP Header** and it contains the **information about the ordering** of the packets and some **information about the packet**.

>- Now, the core idea behind TCP is that when a machine wants to communicate with another machine over TCP like for instance, when a browser, your browser wants to communicate with a website's servers, with AlgoExpert's servers, it's first going to **create a TCP connection with the destination computer/server**.
>- And the way that's gonna happen is through what's known as a handshake.

>- A **Handshake** is a special TCP interaction where one computer basically contacts the other by sending a packet or a few packets saying "*Hey, I wanna connect with you.*"
>- The other computer responds and says, "*Okay, we can connect, we can chat.*" And then the client or the machine that was trying to establish the connection re-responds again and says, "*Okay, we're now connected, we've got an open connection.*"
>- And this is known as a Handshake.

> And then once the connection is established, **both machines can freely send data to one another** but there are few things that might be worth knowing.
>- Like for instance, the fact that if one of the two machines doesn't send data in a given amount of period, the connection can be timed out.
>- If one of the machines wants to end the connection for whatever reason, it can do so by sending some sort of special message to let the other one know that "*Hey, I'm about to end the connection.*" and then the TCP connection is done.

> This is **TCP in a nutshell**.
> To summarize, it is basically a **more powerful**, and **more functional wrapper around IP**,  around the Internet Protocol.
> But still what it **lacks** is a really **robust framework** that developers, software engineers can use to really define meaningful and easy to use communication channels for clients and servers in the system.
> Because with TCP, all that you're really sending is arbitrary data that fits into these underlined IP packets.

> **And this is where HTTP comes into play**.

- **HTTP**
	- HTTP stands for **HyperText Transfer Protocol**.
	- HTTP is **built on top of TCP**.
	- It introduces a **higher level abstraction above TCP** and of course IP.
	- And this abstraction is the **request-response paradigm**.
	- So the HTTP protocol introduces this idea of having machines communicate with one another following this request-response paradigm where one machine sends request to another machine and that other machine returns a response to the first machine.
	- And this request response paradigm with of course a set of accompanying rules makes it very easy for developers to create robust and easy to maintain systems.
	- And so this is why **most modern day systems rely on the HTTP protocol for communication**.
	- So with HTTP, we completely forget about IP packets, we forget about TCP.
	- All that we deal with are HTTP requests and responses.
	- Request are gonna be the things that machines that wanna interact with other machines send.
	- And these request are gonna have a lot of properties defined by the HTTP protocol.
	- And perhaps the best way to really understand or rather appreciate the power and the rigor that HTTP gives you, is to try to visualize what these request and responses look like.
	- One can think of them as objects with important fields or properties that describe them.
	- For example, HTTP Request and Response where requests have fields such as url, port, method, headers, body etc., and responses have fields such as status code, response body, headers etc.

>- If we go back to **IP and TCP**, those two protocols were more **just for transportation of data**.
>- **HTTP** on the other hand introduces the **opportunity to add a lot of business logic** which is of course what you're gonna want if you're developing a large scale system or any kind of system to be honest.

>- **TP**, **TCP** and **HTTP** are **three very important protocols** that basically any modern day system on the internet is gonna be relying on.
>- **IP** and **TCP** are **very very low level** and you're typically not gonna be thinking about them much.
>- **HTTP is more relevant** to you.
>- It's this protocol that's gonna allow you to implement all of the business logic in your system and you have to be familiar with some of these HTTP concepts and terms like requests, responses, methods, path names and so on and so forth.

---

### 5. Storage
> As it turns out, information storage is an incredibly complex topic that is of vital importance to systems design.

#### 4 Key Terms

- ***Databases***
> Databases are programs that either use disk or memory to do do 2 core things: **record** data and **query** data. In general, they are themselves servers that are long lived and interact with the rest of your application through network calls, with protocols on top of TCP or even HTTP.

> Some databases only keep records in memory, and the users of such databases are aware of the fact that those records may be lost forever if the machine or process dies.

> For the most part though, **databases need persistence of those records**, and thus cannot use memory. This means that you have to **write your data to disk**. Anything written to disk **will remain through power loss or network partitions**, so that's what is used to keep permanent records.

> Since machines die often in a large scale system, special disk partitions or volumes are used by the database processes, and those volumes can get recovered even if the machine were to go down permanently.

- ***Disk***
> Usually refers to either **HDD (hard-disk drive)** or **SSD (solid-state drive)**. Data written to disk will persist through power failures and general machine crashes. Disk is also referred to as **non-volatile storage**.

> SSD is far faster than HDD (see latencies of accessing data from SSD and HDD) but also far more expensive from a financial point of view. Because of that, **HDD** will typically be used for **data that's rarely accessed or updated**, but that's stored for a long time, and **SSD** will be used for **data that's freqeuently accessed and updated**.

- ***Memory***
> Short for **Random Access Memory (RAM)**. Data stored in memory will be lost when the process that has written that data dies.

- ***Persistent Storage***
> Usually refers to disk, but in general it is any form of storage that persists if the process in charge of managing it dies.

---

#### Understanding Storage
>- If you think of any system that you might wanna design, you're probably gonna realize that, that **system** is gonna **require some form of storage**. Imagine any system, and that system probably requires some form of storage.
>- Maybe you need to store user information, maybe you need store metrics about the system itself, you'll likely need to store something in that system.

> This is where databases come into play.

- ***Database***
	- A database is a thing, let's call it a thing for now, that really serves two primary purposes:
		- To **store/write/set/record** data
		- To **retrieve/read/get/query** data
	- Now one common **misconception** about databases or rather, a **common gap in knowledge** about databases, is thinking that a database is this magical opaque box that lives somewhere in the ether.
	- And that's really a limited understanding of what a database is.
	- What a database really is, there are of course some exceptions, but what a database almost always is, is just a server.
	- A **database is just a server**. It is just like any other machine/computer.
	- Any machine/computer can genuinely serve as a database for a system. Now that might not be the best decision to make for your system, but the point is it can be.
	- So database is **really just a server**.
	- Now one **very important concept** in storage and in databases is **persistence**.
	- The persistence of the data that you store in a database.
	- A lot of people take for granted or assume, that if they store data in a database, that data will persist through any outage or issue that might occur in your system.
	- People tend to assume that if you store data in a database and then there's a power outage or a network issue or your database server crashes, once everything is booted back up, that the data will still be there.
	- And while that assumption is often fair because a lot of databases do ensure that data stored in them is gonna persist through outages or issues, it isn't always correct.

> And this leads us to two fundamental things in storage: **Disk** and **Memory**

>- If you have a database server, and that database writes data to disk, that data will persist even if the database server goes down.

>- **Writing data to disk** is basically what happens when you save a file on your computer.
>- If you shut down your computer afterwards or if your computer crashes, that file that you saved is still gonna be there unless there's some catastrophic issue with your hardware or some other exceptional issue that data, that file, is still gonna be there.

>- In contrast, if your **database writes data in memory**, and this is what happens when for instance you've got your server code and you have maybe an array or a hash table declared in your server code and you store data in that array or in that hash table if that server goes down, if your database server goes down, and then gets booted back up, the array or the hash table in which you might have stored data is no longer gonna have that data.
>- That's what it essentially means to store data in memory.

>- By the way, if you're wondering why you'd ever want to use memory instead of disk, the simple reason is that **reading data from memory or writing data in memory is much faster than reading data from disk or writing to disk**.

>- Storage is actually a very complex subject area in Systems Design.
>- It's got a lot of depth and a lot of breadth.
>- To give you an idea there are **hundreds of database offerings out there**.
>- If you take Google Cloud Platform alone, it offers eight different storage products.
>- If you're wondering why there's so many database offerings, it's because there are a lot of different things that databases can offer you.
>- For example, database with some kind of structure to store data.
>- Then once we get into **availability**, when we start talking about the uptime of your system, then your choice of database is gonna be really important and different databases are gonna give you different things.
>- You can imagine if your database goes down, because your database is such a critical part of your system, then your entire system effectively goes down with your database if it goes down.

> And so then this brings us to the topic of **distributed storage**.
>- Because so far we've only talked about storing data on one machine.
>- But if you don't want your entire system to get brought down when your database goes down, then you're probably gonna need to store your data not on one machine but on multiple machines and that comes with a lot of complexity.

>- Then we start asking questions like, "*Well how do you store data on multiple machines?, Do you split the data up?, Do you replicate the data across multiple machines?"* then this leads us to consistency issues.

>- **Consistency** is a concept in storage that basically refers to the staleness or the up-to-dateness of data.
>- For instance if you access data from a database, especially if that database is distributed across multiple machines, are you ever gonna get stale data or will you always get the most up-to-date version of that data?
>- That's consistency in a nutshell.

>- And here this is where those hundreds of database offerings are gonna come into play because some databases are gonna give you certain properties or certain guarantees but they're gonna trade off others and other databases are gonna give you different properties in exchange for other trade-offs.

---

### 6. Latency And Throughput
> If you've ever experienced **lag** in a video game, it was most likely due to a **combination of high latency and low throughput**. And lag sucks.

#### 2 Key Terms

- ***Latency***
> The **time it takes for a certain operation** to complete in a system. Most often this measure is a time duration, like milliseconds or seconds. You should know these orders of magnitude:
>- ***Reading 1 MB from RAM:*** 250 μs (0.25 ms)
>- ***Reading 1 MB from SSD:*** 1,000 μs (1 ms)
>- ***Transfer 1 MB over Network:*** 10,000 μs (10 ms)
>- ***Reading 1 MB from HDD:*** 20,000 μs (20 ms)
>- ***Inter-Continental Round Trip:*** 150,000 μs (150 ms)

> And there are a **million microseconds** in **1 second**.
> **10<sup>6</sup> microseconds** in **1 second**.

- ***Throughput***
> The **number of operations that a system can handle properly per time unit**. For instance the throughput of a server can often be measured in requests per second (RPS or QPS).

---

#### Understanding Latency And Throughput
>- Latency and throughput are two things that are **extremely important in the context of systems design interviews**.
>- They're actually **not that difficult** to grasp.
>- But they are often misunderstood. Because a lot of people actually know the terms latency and throughput. They might even use them in sentences every so often. But, a lot of people also don't quite understand exactly what the two words mean.
>- Latency and throughput are the **two most important measures of the performance of a system**.

- ***Latency***
>- **Latency**, to put it simply, is basically **how long it takes for data to traverse a system**. And more specifically, how long does it take for data to get from one point in a system, to another point in a system.
>- When talking about **latency**, we might refer to a lot of **different kinds** of things **in a system**.
>- **For instance**, we might be talking about the **latency of a network request**. How long does it take for one request to go from a client to a server, and then back from the server to the client ?
>- We would refer to the time that it takes for a request to go from a client to a server, and then back from the server to the client as latency.
>- The time that it's gonna take to **read data from memory or disk** is also gonna be referred to as latency.
>- The most important aspect of latency is the fact that these **different things in systems, have different latencies**.
>- And so basically **there's a trade off** between different ways that a system is built.
>- Because certain things are gonna have higher latencies, and other things are gonna have lower latencies.

> Examples of latencies of various operations is mentioned in the [key terms section](https://github.com/Harishankar-GitHub/SystemsExpert/tree/main/Systems%20Design%20Fundamentals#2-key-terms).

>- When you are gonna be designing systems, you're typically going to **optimize those systems**, by lowering the overall latencies of the systems.
>- Some systems will not warrant optimizing for latency as much as others.
>- For instance, you could imagine that certain types of systems might really, really care about having low latencies. A good example here is video games.
>- If you've ever played an online video game, especially a multiplayer video game where you're competing against people or playing with people.
>- When we talk about lag in those types of video games, what we really mean is, those video games or those systems have a high latency, or you as a player have a high latency.
>- And that might literally be because the server that you're playing on is located halfway across the world from you, and it just takes a while for your computer, the client, to make a network requests to the video games server.
>- And even though 150,000 microseconds **seems really fast**, you could imagine that if you're sending a lot more data over the network, then these 150,000 microseconds **quickly add up** and if you're **playing a video game** where you need almost **instantaneous actions**, or things to happen, then this is gonna be a really bad experience for the user, and so you're gonna have designed your system really poorly if you have high latency.

>- On the other hand, you might imagine certain websites that might care less about latency because maybe they don't really care if it takes a couple seconds for the page or the website to load.
>- But what they care about more is maybe accuracy or up time.
>- They want their website to always show accurate information, or never to be down. But they're okay to lose some latency.

>- **When tackling System Design interviews**, you're gonna have to **think of** these kinds of **trade offs**, or the kinds of **priorities** that you have when you're designing a system.
>- **And latency is something that you're definitely going to consider**.

- ***Throughput***
>- **Throughput** is **how much work a machine can perform in a given period of time**.
>- And so typically, at least in the context of System Design interviews, but also in computing in general.
>- When we talk about throughput, and we talk about this amount of work that a computer or machine can perform in a given amount of time, we're really referring to how much data can be transferred from one point in a system to another point in a system, in a given amount of time.
>- And so typically, we **measure** this throughput, in **gigabits per second**, or **kilobits per second**, **megabits per second**.
>- **For example**, transferring 1 MB over 1 Gbps Network literally means that this network can support 1 gigabit per second or a billion bits per second.

>- A good way to think about throughput is with an image, if a lot of clients are requesting an image from a server, and they're all issuing requests to the server, the throughput is basically gonna be how many of these requests can this server handle in a given amount of time, or in this case a second.
>- And more specifically if we reduced these requests to bits, how many bits can this server handle or let through per second?
>- You could almost imagine that this is kind of like a bottleneck where you can only fit so many bits during a given amount of time, again in this case seconds, and that's throughput.

#### How to increase throughput ?
>- So how to increase throughput or how do I optimize a system for throughput?
>- And so the simple answer, perhaps even the naive answer is, **you just pay for it**. You pay to increase throughput.
>- Well, if you take a look at AlgoExpert for example, the thing that determines how many bits can go in and out of AlgoExpert's servers, at any given time, or during a second for instance, is determined by the cloud provider, which happens to be Google Cloud Platform, Google in this case.
>- So basically we can pay Google, or at least in theory we can pay Google to just increase throughput.

> **Just increasing throughput doesn't necessarily fix a potential problem that you might have in a system**.

>- As an example, imagine we have a system, where we have just a single server, that's handling request from tons of different clients.
>- You could imagine that this system might be a system like, Google Search or Facebook Messenger, that might expect to serve thousands of requests, perhaps even millions of requests per second.
>- And just trying to blindly increase throughput on this network probably won't make sense because you'll still eventually have some sort of bottleneck here.
>- So perhaps a better way to fix this system would be to have multiple servers handle all these requests.
>- And that might be a better way to design the system.

>- **One last thing** that's important to mention **about latency and throughput**, is that even though they are very much related in a way, and they're very important measures of a systems performance, **they're not necessarily correlated**.
>- For instance, you might have a system, or rather parts of a system, smaller parts of a system, that have very low latency.
>- In other words, they support really fast data transfers.
>- But then you might have a part of the system that has very low throughput, and so that ends up meaning that the low latency data transfers or operations that the system had, are kind of cancelled out.
>- In other words, you can not make assumptions about latency or throughput based on the other.
>- They are not necessarily correlated things.

---

### 7. Availability
#### 3 Prerequisites
- ***Process***
> A program that is currently running on a machine. You should always assume that any process may get terminated any time in a suffeciently large system.

- ***Server***
> A machine or process that provides data or service to a client, usually by listening for incoming network calls.

> Note that a single machine or piece of software can be both a client and a server at the same time. For instance, a single machine could act as a server for end users and as a client for a database.

- ***Node/Instance/Host***
> These three things refer to the same thing most of the time: a virtual or physical machine on which the developer runs processes. Sometimes the word **server** also refers to the same concept.

#### 6 Key Terms

- ***Availability***
> The odds of a particular server or service being up and running at any point in time, usually measured in percentages. A server that has 99% availability will be operational 99% of the time (this would be described as having **two nines** of availability).

- ***High Availability***
> Used to describe systems that have particularly high levels of availability, typically **5 nines or more**; sometimes abbreviated "**HA**".

- ***Nines***
> Typically refers to percentages of uptime. For example, 5 nines of availability means an uptime of 99.999% of the time. Below are the downtimes expected per year depending on these 9s:

```
- 99% (two 9s): 87.7 hours
- 99.9% (three 9s): 8.8 hours
- 99.99%: 52.6 minutes
- 99.999%: 5.3 minutes
```

- ***Redundancy***
> The process of replicating parts of a system in an effort to make it more reliable.

- ***SLA***
> Short for "**service-level agreement**", an SLA is a collection of guarantees given to a customer by a service provider. SLAs typically make guarantees on a system's availability, amongst other things. SLAs are made up of one or multiple SLOs.

- ***SLO***
> Short for "**service-level objective**", an SLO is a guarantee given to a customer by a service provider. SLOs typically make guarantees on a system's availability, amongst other things. SLOs constitute an SLA.

---

#### Understanding Availability
>- When evaluating a system, two of the things that you wanna think about are the system's latency and the system's throughput. And that's certainly true.
>- But there's another thing that you wanna think about and that's the system's availability.

- ***What is Availability?***
>- **One way to think** about it is how resistant a system is to failures.
>- For instance, what happens if a server in your system fails? What happens if your database fails?
>- Is your system gonna completely go down or your system still gonna be operational?
>- And this is often described as a system's fault tolerance, how fault tolerant is a system.

>- **Another way to think** about availability is, as the percentage of time in a given period of time, like a month or a year, are at least operational enough such that all of its primary functions are satisfied.

> **Availability is a very important thing to think about when evaluating a system.**

>- And in this day and age, especially, **most systems almost have an implied guarantee of availability**.
>- An example of this would be AlgoExpert. If you take AlgoExpert, the website, the product, the platform, when someone purchases AlgoExpert, the main thing that purchased is the access to the platform, access to the content, the ability to watch the videos.
>- But if you think about it, there's an implied guarantee of availability that comes with the purchase of AlgoExpert.
>- Because if you are a customer and go to the [website](algoexpert.io) you expect the website to be up and you expect the website to be fully operational.
>- If the website ever isn't fully operational, you are not gonna be happy.
>- This not only makes the customer unhappy, but also make the company lose money.
>- This is just one example.

> **There are varying degrees of availability that you might expect from different systems.**

>- In the case of AlgoExpert, if the website were down for a few hours or if parts of the platform weren't operational for a few hours, well, it would be upsetting for customers. And while it would be bad for the service providers, it wouldn't really be the end of the world, it wouldn't be the most unacceptable thing to ever happen.
>- Now imagine that we were dealing with a system that supported airplane software, the software that allows an airplane to function properly when it's in flight.
>- You could imagine that if that system were to ever go down when an airplane were flying, that would be absolutely unacceptable.
>- So in that type of system, you would expect an extremely high amount of availability.
>- Any amount of complete downtime in the system would just be unacceptable.
>- And by the way, here we don't necessarily have to reach so far into life or death examples like airplane software.
>- You can take a step back and look at platforms like YouTube. If YouTube ever goes down, that's really bad because hundreds of millions of people use YouTube everyday.
>- Or take cloud providers, for instance. Take cloud providers like Google Cloud Platform or Amazon Web Services.
>- If parts of these cloud providers' systems ever go down, that can be really bad because it then affects all of the businesses and customers that rely on their services for their own platforms.

>- **As an example**, in the summer of 2019, in June or July, Google Cloud Platform had a really bad outage that affected a bunch of its products and services.
>- This outage lasted at least a couple of hours. Many or all of the businesses that relied on Google Cloud Platform were affected.
>- So, for instance, Vimeo, which apparently runs on Google Platform, at least in part, was affected.
>- This meant that people on AlgoExpert couldn't watch our videos because our videos are hosted on Vimeo. And AlgoExpert received something like 10 customer messages in the span of one hour saying, _"Hey, how come I can't watch videos? Are the videos down? Is there a problem?"_
>- And so as you can imagine, this was just really bad all around.
>- One outage on Google Cloud Platform has huge and far-reaching repercussions.

> **All that to say that availability matters a lot.**

- ***How do you measure Availability?***
>- What does it mean for a system to be available?
>- Well, it turns out that we typically measure availability as the **percentage of a system's uptime in a given year**.
>- So, for instance, if a system is up and operational for half of an entire year, then you would say that that system has **50% availability**.
>- Now, in practice, you could imagine that 50% availability would be really, really bad for most services.
>- Imagine if Facebook were down 50% of the year. Imagine if Uber were down 50% of the year. That would not be acceptable. These products would never survive in the market.
>- So when we're dealing with availability, we're usually dealing very, very high percentages.
>- In fact, it can be pretty deceptive because even an **availability of 90% isn't really great**.
>- If you do the math, 90% means that your system is gonna be down about 35 or 36 days out of the year.
>- Again, imagine if Facebook or Uber were down 36 days out of the year. They would never survive in the marketplace.

> So what that means is that in the industry, most services or most systems aim for really high availabilities and so we often end up measuring availability not exactly in percentages but rather in what we call **nines**.

>- **Nines** are effectively percentages but they are specifically percentages with the number nine.
>- If you have a system that has **99%** availability, meaning that it is up 99% of the time during a year.
>- Then, in the industry, we say that your system has **two nines** of availability because literally the number nine appears two times in this percentage.
>- If your system has **99.9%** availability, then we say that it has **three nines** of availability.
>- If it has **99.99%**, then we say it has **four nines** of availability and so on and so forth.
>- And this is really the standard way that people talk about availability in the industry.

> [High Availability - Wikipedia](https://en.wikipedia.org/wiki/High_availability)

>- **Five nines** of availability is typically regarded as the **gold standard of availability**.
>- If your system has five nines of availability, then we would really say that it is a highly available system.
>- And by the way, that's an actual term.
>- Calling a system highly available or saying that a system has high availability is an actual **recognized term in systems design**.
>- And it's often abbreviated as **HA** for **high availability** or **highly available**.
>- So a lot of systems aim to be highly available systems because they really care about availability, they really care about having a high level of availability, they wanna shoot for that ideal five nines of availability, maybe even more.
>- And so we say that they wanna be highly available systems or if the actually have that kind of availability that they are highly available systems.

> **Availability is really important and it's something that matters a lot both to the end users of systems and to systems designers.**

>- In fact, it matters so much that for certain systems, they don't have an implied guarantee of availability, they have an **explicit guarantee of availability**.
>- Many service providers out there have what are known as **SLAs**.
>- **SLA** stands for **service-level agreement**.
>- SLA is an agreement between a service provider, basically the people who are behined the service or system that is being sold or provided, and the customers or end users of this service or of this system, **an agreement on that system's availability** amongst other things.
>- So many service providers out there have these explicit written SLAs, service-level agreements, that basically tell customers, _"Hey, we guarantee you this amount of availability. This percentage of uptime, for instance, in our system."_
>- **SLO**, which is often used synonymously with SLA in the industry but that's incorrect because SLO is not the same thing as SLA, it's related but not the same thing.
>- **SLO** stands for **service-level objective**. 
>- SLO can be considered as components of SLA.
>- In other words a **service-level agreement is made up of service-level objectives**.
>- If a provide a service for you and I guarantee you a percentage of uptime for that service, for example, that percentage of uptime guarantee would be an SLO.
>- If I guarantee you that you will only get X number of errors when you use my service, and here let's just imagine that we're talking about arbitrary errors, then that is another SLO.

>- And so all these major cloud service providers, for example, like Google Cloud Platform or Amazon Web Services have very clearcut SLAs.
>- In fact, you can actually see them online on their product pages.
>- And these are very important when you're considering buying their services because depending on your use case and your need for their services, you might require some percentage of availability.
>- And so you're gonna want something very clearly and unambiguously specified in an SLA to give you that peace of mind.

> SLAs are very serious and availability is taken very seriously, which means that availability is extremely important in systems design and of course in systems design interviews.

>- Even though availability is something to be taken very seriously and is really valued when designing a system, **it's not always super important** or it's not always the case that you need to have five nines of availability.
>- Because having **high availability comes with trade-offs**.
>- It's **difficult to achieve** high availability.
>- And so you, as the systems designer, have to think long and hard about whether or not your system should be highly available.
>- You have to think long and hard about what parts of your system should be highly available or don't need high availability.
>- **Stripe** is a very popular product that provides, amongst other things, payment services for businesses.
>- So, for instance, AlgoExpert relies heavily on Stripe. All of their credit card processing and all of their payments, basically, that don't use PayPal are done through Stripe.
>- And so if you take a service like Stripe and you dissect it a little bit, you can start to understand what parts of a system do require high availability and what parts of a system don't necessarily require the same levels of availability.
>- For Stripe, you could imagine that their core services of handling payments and of charging customers, that is likely a highly available service.
>- If that service would ever go down, that would be really bad and their customers could lose thousands if not millions of dollars of revenue. They could lose millions of dollars of revenue, so that part of their system probably has to be highly available.
>- But then other parts of their system might not have to be highly available.
>- For example, they have a dashboard that businesses can use to monitor their sales. That dashboard is not as critical as the core payment service that Stripe provides.
>- If that dashboard goes down, that's still pretty bad but it's not the end of the world, it's not outrageous.

>- When designing systems, in systems design interviews or even on the job, you're gonna have to ask yourself: _"What parts of my system are absolutely critical?"_ Well, not necessarily critical but are critical to the point that they require high availability.
>- And what parts of my systems don't actually require high availability?
>- What parts of my systems would be okay to fail?
>- That's gonna be something that you'll have to think about.

- ***How do you improve Availability?***
>- It's really conceptually quite simple.
>- You wanna **make sure**, first and foremost, that your **system doesn't have single points of failure**: Single places in your system that if they fail cause your entire system to fail.
>- And how do you **eliminate single points of failure**? Answer is **Redundancy**.
>- **Redundancy** is basically the act of duplicating or triplicating or multiplying even more certain parts of your system.
>- So, as an example, if you've got a very simple system where you've got clients that interact with your server, then your server interacts with a database, you can clearly see that this single server here is a single point of failure.
>- If this single server gets overloaded or if there's a problem with it for whatever reason and it dies, then your entire system fails.
>- So what would you wanna do? You would wanna make this part of your system redundant.
>- And you would do so by basically adding servers.
>- Now, if you add servers, you probably wanna have a load balancer in between your clients and your servers to distribute the load of your clients across your three servers.
>- What if your load balancer becomes overloaded? Now your load balancer is a single point of failure.
>- And so you can have redundancy at the load balancer layer in your system.
>- For example, on AlgoExpert, it has 5 load balancers that take in all of the user traffic and then forward that traffic to the servers.
>- The point is that you can introduce redundancy in a lot of different parts of your system just by literally adding machines to those parts of your system.
>- **This is known as Passive Redundancy.**

- ***Passive Redundancy***

>- Passive redundancy is loosely speaking when you have **multiple components at a given layer in your system**.
>- And if at any point one of those components, like, for instance, one of these servers or one of these load balancers, if at any point in time one of them dies, nothing's really gonna happen.
>- The other two servers or the other two load balancers are basically gonna be able to continue running smoothly.
>- They might have a little bit more load but they'll be fine until the broken load balancer or the broken server gets fixed.
>- And here an example of passive redundancy that's often used is airplane engines.
>- When you're dealing with a twin engine airplane, an airplane that has two engines, both engines are being used, but if one engine fails, it gets completely broken, the airplane can still fly completely smoothly and even land and take off with just one engine.
>- So that's an example of passive redundancy.

- ***Active Redundancy***
>- Active redundancy is a little bit more complicated.
>- Active redundancy is when you have multiple machines that work together in such a way that only one or few of the machines are gonna be typically handling traffic or doing work.
>- And if one of the ones that is handling traffic or doing work fails, maybe it's the only one handling traffic or doing work, and it fails, **the other machines are gonna somehow know that that other one failed and they're gonna take over**.
>- This is known as active redundancy.

>- If you wanna make a system available or even highly available, you're gonna need to eliminate single points of failure in that system, and you can do so by making these parts of your system redundant.
>- And of course it's important to mention that you'll also wanna make sure that you **have a rigorous processes in place to handle system failures** because it's possible that system failures are gonna require human intervention.
>- Maybe if servers in your system crash, you're gonna need a human to bring them back up.
>- And you're gonna need to have processes in place that ensure that that happens in the proper timeframe.
---

### 8. Caching
#### 5 Key Terms
- ***Cache***
> A piece of hardware or software that stores data, typically meant to retrieve that data faster than otherwise.

> Caches are often used to store responses to network requests as well as results of computationally-long operations.

> Note that data in a cache can become **stale** if the main source of truth for that data (i.e., the main database behind the cache) gets updated and the cache doesn't.

- ***Cache Hit***
> When requested data is found in a cache.

- ***Cache Miss***
> When requested data could have been found in a cache but isn't. This is typically used to refer to a negative consequence of a system failure or of a poor design choice. For example:

> If a server goes down, our load balancer will have to forward requests to a new server, which will result in cache misses.

- ***Cache Eviction Policy***
> The policy by which values get evicted or removed from a cache. Popular cache eviction policies include LRU (least-recently used), FIFO (first in first out), and LFU (least-frequently used).

- ***Content Delivery Network***
> A **CDN** is a third-party service that acts like a cache for your servers. Sometimes, web applications can be slow for users in a particular region if your servers are located only in another region. A CDN has servers all around the world, meaning that the latency to a CDN's servers will almost always be far better than the latency to your servers. A CDN's servers are often referred to as **PoPs** (Points of Presence). Two of the most popular CDNs are Cloudflare and Google Cloud CDN.

---

#### Understanding Caching
>- Caching is one of the important topics or techniques in Systems Design.
>- In fact, you're likely going to be using caching in all, or almost all, of your Systems Design interviews.
>- Caching is **used in a lot of algorithms**.
>- The **reason** is to typically **avoid redoing the same operations**, especially computationally complex operations that might take a lot of time, multiple times.
>- So caching is **used to improve the time complexity of the algorithms**, to speed up the algorithms.

>- And **in the context of systems design**, caching is actually pretty similar.
>- To put it simply, caching is used to speed up a system.
>- Caching is **used to reduce or to improve the latency** of a system.
>- Caching is going to be a way to design a system in such a way that, if we were originally gonna be using types of operations or data transfers that take a lot of time, like for example, network requests, we're gonna design a system in such a way that we don't have to do those network requests, and we can do different types of operations or different types of data transfers that are going to be faster.
>- A much simpler way to put it is, caching is gonna be storing data in a location that's different from the one where the data originally is, such that it's faster to access this data from this new location.

>- **Caching can be used in a bunch of different places in a system**.
>- For instance, you can cache at the **client level**. So that the client caches some data such that it no longer has to go to the server to retrieve it.
>- Similarly, you could cache at the **server level**. Maybe you need the client to always interact with the server, but maybe the server doesn't always need to go to the database to retrieve data. Maybe it only needs to go to the database once and we can have some form of cache here at the server level.
>- You could also have a **cache in-between two components** in a system. So maybe you could have a cache in-between a server and a database.
>- In fact, you can even have **caching at the hardware level**. Now, perhaps this is less important in the context of Systems Design interviews, but it's still good to know about this.
>- There is actually a lot of caching that happens at the hardware level in modern-day computers.
>- For example, there's CPU caches, which are caches, as the name implies, that live at the CPU level, that basically make it faster to retrieve data from memory.

> **It is good to know that caching can occur, or occurs by default, at many different levels of a system.**

#### Concrete instances where caching is really helpful
> The **first instance** where caching is gonna be really helpful is if you're doing a lot of network requests and you basically wanna avoid doing all of these network requests.

> **Another instance** where caching is very helpful is if you're doing some very computationally long operation. So perhaps it's not the network request that you're trying to avoid doing, but some other computationally long operation.

> In both of these cases, the goal behind the caching is to speed up the system.

>- **But there's another instance** where caching is gonna be very useful, and it's not necessarily gonna be to speed up the system in that case.
>- Imagine that you had multiple servers and all of these servers were hitting the database.
>- They all hit the database with the same network requests that this first server does.
>- Maybe you've got a bunch of clients that are all doing the same thing, maybe they're all making individual requests to different servers to get a certain Instagram profile for instance.
>- Let's say there's a popular celebrity and you've got a million users who are trying to view that popular celebrity's Instagram profile.
>- Here you can use caching not so much to increase the speed of each network request when it's trying to get the profile, cause that's not necessarily something you need to optimize on, an individual network request would be very quick, but maybe you don't want to read from the database a thousand times or a million times because that might overload the database for instance.
>- So, you would use caching to not have to read from the database that many times.

>- So these are three very good examples of when you might want to use caching in a system. Either to speed up an operation that involves a network request by avoiding having to do the network request all together, or at least avoiding having to do it multiple times.
>- Maybe you want to speed up an operation because it's computationally long, and so you just cache the results so that you don't have to do that computationally long operation.
>- Or maybe you have an operation that's done tons of times, you don't necessarily need to speed them up individually, but you just don't wanna perform it that many times because it might affect your system in other ways, and you might wanna use caching there.

#### Concrete examples of caching in action
>- **First example** is on **AlgoExpert**.
>- If you go on AlgoExpert and you go to the questions list on AlgoExpert, the list of coding interview questions, you might notice that the first time that you go on that page there's going to be a loader.
>- There's going to be a little loading icon and depending on how fast your internet connection is, you might see that loading icon for just a split second or for a few seconds.
>- Now if you go to another page afterwards, you don't close your browser or your tab but just go to another page, and then you go back to that same questions list, you'll notice that the icon is no longer there and the questions list is almost pre-loaded.
>- It's like it's there on the page immediately.
>- Why is that the case? Because of caching.
>- AlgoExpert caches the questions list on the client.
>- Because AlgoExpert knows that the questions list is a static piece of content, it's the same every time that you get it, or at least if we put aside you know, marking questions as completed or changing the order of questions, that adds a little bit of complexity.
>- But the questions list is static content. It's the same every time.
>- And so instead of having the user or the client make a network request to our server every time that they go on the page to see the questions, we just cache the result on the client after the first time that we make the network request and that way you just get a faster experience on the website.

>- So **another concrete example** of caching would be when you're **running code on AlgoExpert**.
>- So running code on AlgoExpert takes, on average, about one second.
>- There's a lot of stuff behind the scenes so it takes a non-trivial amount of time.
>- Now as you can imagine, when people run code on AlgoExpert with AlgoExpert's solutions, that don't change no matter what user is running them, AlgoExpert doesn't need to do that one second computation every time.
>- What they can do instead is cache the results for running code with AlgoExpert's solutions, and when users do that AlgoExpert just return to them the values that are in our cache.
>- And that's going to be much faster. That's going to be on the order of milliseconds rather than one full second, or even more.
>- And so here, by the way if you're wondering _"well how do you cache the result of running code?"_ because when you're running code you're making a network request, where would you store the cache?
>- Well you might store the cache at the server level or maybe detached from the server in some independent component.
>- And here you might use something like Redis, which is a very popular in-memory database, it's actually a key value store.
>- But so the way that this caching would work is the client, meaning you the user, would go on AlgoExpert on the coding workspace, you would run code with one of AlgoExpert's solutions.
>- This would send an http request to AlgoExpert servers. Then what AlgoExpert servers would do is they would say, _"hey we've got this request which is just a bunch of bytes."_
>- AlgoExpert is gonna hash it down, gonna hash this request, these bytes down to a single signature, very much like a hash table.
>- So they might hash it down to, for instance, an integer. And then they'd check the cache, which might either be in memory on the server or in some detached component, like Redis for instance which is a key value store, and we check if the key is in the cache.
>- If it is they take the value associated with that key and they return it to the client.
>- And so AlgoExpert has avoided doing that additional one second computation of actually running the code and they've just used the value that they had in the cache.

>- Okay, but so far all the examples of caching that we've looked at involve storing data that only needs to be read not data that needs to be written.
>- Let's imagine that we were designing a system, or a web application, where users can read and write posts and they can edit their posts.
>- So you can imagine writing Facebook posts or writing LinkedIn posts.
>- So you can image that you'd have a client, the browser that you the user are interacting with. Then you'd have a server.
>- So when you're a user who's writing a post you make a request to the server to write the post and then the posts are stored in a database.
>- But now if you wanna cache those posts, let's say that you're caching the posts at the server level in memory.
>- You now have two sources of truth. Your posts are stored both in the database and in the server.
>- So let's say that you edit a post. You're the user, you've written a post, so behind the scenes what happened is that the client made a network request with your new post, the server made a network request to the database and stored the post in the database.
>- And then you wanna display that post on the page and somehow the post got stored in the cache, how do you deal with these two sources of truth and how do you know when you write to the cache for instance, when to write to the database? You do that at the same time? Do you not do that at the same time?
>- Well here we're gonna cover two popular types of caches.
