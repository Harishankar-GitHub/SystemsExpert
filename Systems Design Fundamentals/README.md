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
>- If you go on AlgoExpert and you go to the questions list on AlgoExpert, the list of coding interview questions, you might notice that the first time that you go on that page there's going to be a loader (The icon that appears near the tab name when the page loads).
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
>- And then AlgoExpert is gonna hash it down, gonna hash this request, these bytes down to a single signature, very much like a hash table.
>- So they might hash it down to, for instance, an integer. And then they'd check the cache, which might either be in memory on the server or in some detached component, like Redis for instance which is a key value store, and we check if the key is in the cache.
>- If it is they take the value associated with that key and they return it to the client.
>- And so AlgoExpert has avoided doing that additional one second computation of actually running the code and they've just used the value that they had in the cache.

>- Okay, but so far all the examples of caching that we've looked at involve storing data that only needs to be read, not data that needs to be written.
>- Let's imagine that we were designing a system, or a web application, where users can read and write posts and they can edit their posts.
>- So you can imagine writing Facebook posts or writing LinkedIn posts.
>- So you can image that you'd have a client, the browser that you the user are interacting with. Then you'd have a server.
>- So when you're a user who's writing a post you make a request to the server to write the post and then the posts are stored in a database.
>- But now if you wanna cache those posts, let's say that you're caching the posts at the server level in memory.
>- You now have two sources of truth. Your posts are stored both in the database and in the server.
>- So let's say that you edit a post. You're the user, you've written a post, so behind the scenes what happened is that the client made a network request with your new post, the server made a network request to the database and stored the post in the database.
>- And then you wanna display that post on the page and somehow the post got stored in the cache, how do you deal with these two sources of truth and how do you know when you write to the cache for instance, when to write to the database? You do that at the same time? Do you not do that at the same time?
>- Well here we're gonna cover two popular types of caches.

- ***Write Through Cache***
>- A write through cache is a type of caching system where when you make an edit to a piece of data, when you write a piece of data, your system will write that piece of data both in the cache and in the main source of truth (Database) at the same time, or rather in the same operation.
>- So here for instance, let's say that you have a post, your post is stored in the database, it's also stored in your cache, and you're a user and you want to make an edit to that post, You're gonna make a network request to the server and the server is gonna overwrite whatever is in the cache and then it's also gonna make the request to the database and overwrite what's in the database.
>- That way the **cache and the database are always in sync**.
>- Now the down side to this is that you end up having to still go to the database, whereas in some of the previous examples of caching we were able to avoid certain network calls and certain operations, here with this kind of write through caching every single time you're gonna overwrite something in the cache or in the database you're gonna be doing two things, and you're still gonna be going to the database.
>- So this brings us to the second popular type of cache.

- ***Write Back Cache***
>- A write back cache behaves a little bit differently.
>- Let's say again that you're a user, you're editing your post.
>- You're gonna make a network request to the server, and the server's gonna update the cache but only the cache.
>- And it's gonna immediately go back to the client.
>- And so now your **cache will actually be out of sync with your database**.
>- And what'll happen behind the scenes is that your **system will asynchronously update the database with the values that are stored in the cache**.
>- And **this can be done in different ways**.
>- Maybe it's on certain intervals, so maybe every five seconds, every five minutes, every five hours. Who knows.
>- Or maybe it's gonna be following a different type of schedule.
>- Maybe it'll be whenever your cache gets filled up and you have to evict stuff out of the cache.
>- But so, the point is, with a write back caches in this example whenever the user makes a network request to the server to edit their post, only the cache will be updated, and then at some other point asynchronously the database is gonna get updated.
>- Now you can image that one of the downsides here is that if something ever happens to your cache and you lose the data in the cache, for instance, before the database has been updated asynchronously, then you're gonna lose data and that's really bad.
>- But of course there might be ways to mitigate that.
>- Now where things get tricky is when you're dealing with very large systems that might have a lot of different components.

>- Let's assume that we've been charged with designing the YouTube comments section system.
>- And we've decided that we've got a bunch of servers.
>- Every server caches in memory the comments on a single video.
>- And then we've got all of our clients that communicate with the respective servers, and when they're reading comments, they just read from the caches in their respective servers.
>- So now let's assume that our first client has posted a comment on the video and our second client goes to the video.
>- The server goes to the database first to fetch all the comments and stores them in cache, and then some time elapses, the clients do kind of whatever, and then eventually this client goes back and edits it's comment.
>- So the user behind the client edits their comment.
>- And then the second client goes back to the video but this time the server doesn't go to the database because it has the comments already stored in memory, cached in memory.
>- And so the second client sees the old version of the first client's comment, not the newly edited one.
>- And second client responds to that old comment, not the newly edited one.
>- As you can imagine, that would be really bad from a product point of view.
>- That would likely be unacceptable for something like YouTube comments.
>- You don't want people to be responding to older versions or stale versions of comments.
>- And of course this applies to any written content. Things like posts would definitely fall into this category.
>- So here we are getting into the concept of **Staleness**.
>- **Caches can become stale if they haven't been updated properly**.
>- So here, this particular system the way that we've designed it, would be really bad because our clients would often be dealing with stale caches, or rather with caches that hold stale data, and that would not be good.
>- In this particular system, **perhaps a solution would be to move our cache out of the servers and to put our cache, a single cache**.
>- Maybe this would be **Redis**.
>- And all of the servers would hit the cache and we'd have this single source of truth for the caching mechanism.

>- **On the other hand** you might imagine that for certain parts of our system, or rather certain features that we're trying to build out with our system, we might actually not care that much about the staleness or non-staleness of the data in our caches.
>- As an example, let's take view count on YouTube videos.
>- View count isn't necessarily the most important piece of information on a YouTube video.
>- And if one user sees a slightly stale version of a view count on a video, that's probably not gonna be the end of the world.

> **So this is the kind of stuff that you need to start asking in a Systems Design interview and you obviously have to work with your interviewer here and ask them questions.**

- **Few questions**
	- ***"What are the things that we're trying to build out?"***
	- ***"What are the requirements?"***
	- ***"Do we care about the accuracy of data that much?"***
	- If we do, for things like posts where we definitely don't wanna be answering/replying to posts that have been edited but we don't see the edit because we're seeing a stale version of that data, then we might not be able to use caching in a naive way.
	- But if it's the kind of data where we don't really care if it's stale, then maybe we can use caching in a more naive way like we had it originally, and that'll be fine.

>- So the summary here is that caching, while it's great, has a lot of pitfalls. And you have to watch out for those pitfalls.
>- In general, if the data that you're dealing with is static data, or immutable data, like for instance the questions list on AlgoExpert, then caching is beautiful and it typically works very easily.
>- But if you're dealing with data that is mutable then things are gonna be trickier because you're gonna have two different locations where the data exists, you're gonna have to make sure that these locations are in sync otherwise the data might become stale, and depending on your use case that might not be good.

>- So as a **rule of thumb**, you should definitely **consider caching** if you're only storing immutable data or static data.
>- You should consider using caching if you're only gonna have a single thing reading or writing that data, because the second that you introduce multiple things reading or writing data then things become a little bit more complex.
>- If you don't care about consistency, if you don't care about the staleness of data, then you can totally consider caching because you might not have to worry about the potential pitfalls of caching.
>- Or, if you're able to design your system in such a way that you can properly invalidate or get rid of stale data in your cache or in your caches, especially in a distributed manner if you're dealing with a distributed system, then caching is certainly gonna be something you're gonna wanna consider.

- ***Eviction Policies In Caching***
>- As you can imagine, not only do we not have infinite space, so you can't store an infinite amount of data in a cache, but also sometimes you're gonna be left with stale data in your cache and you're gonna wanna get rid of that stale data.
>- And so this is where we get into eviction policies.
>- How do we actually get rid of data in caches, or rather what policy or rules do we follow to get rid of data in caches?
>- And here there are a **few popular rules or a few popular policies**.
>- One that you may have heard of from coding interviews, because it's a popular coding interview question, the LRU policy.
>- The **Least Recently Used policy**.
>- Basically what that means is you get rid of the least recently used pieces of data in a cache and you have some way of tracking what pieces of data are the least recently used.
>- Because basically you make the assumption that the piece of data that was used least recently is likely the one that we no longer care about, or that we least care about.
>- There's also the **Least Frequently Used policy** where you have a bunch of data in your cache, the least frequently used of that data, not necessarily the least recently used, but the least frequently used is the one you get rid of.
>- You could also get rid of data in your cache in a **last in, first out or a first in, first out basis**.
>- Or **even just randomly**.
>- The point is **there's lots of ways to evict data from a cache**, and here this is something **that's gonna depend on your use case**, on the **product or the system** that you're building or designing.

> **And here you would obviously have to talk with your interviewer to figure out what things are valued**.
---

### 9. Proxies
> Often used by nefarious hackers to conceal their identity and obfuscate their location, these special intermediary servers boast many important real-life applications within the context of caching, access control, and censorship bypassing, amongst other things.

#### 3 Key Terms
- ***Forward Proxy***
> A server that sits between a client and servers and acts on behalf of the client, typically used to mask he client's identity (IP Address). Note that forward proxies are often referred to as just proxies.

- ***Reverse Proxy***
> A server that sits between clients and servers and acts on behalf of the servers, typically used for logging, load balancing, or caching.

- ***Nginx***
>- Pronounced "engine X", not "N jinx". Njinx is a very popular webserver that's often used as a **reverse proxy** and **load balancer**.
>- Learn more [https://www.nginx.com/](https://www.nginx.com/)

---

#### Understanding Proxies
>- In the industry, it turns out that people use the term proxy pretty loosely and when they use the term proxy, they often mean forward proxy.
>- They just don't mention the word forward, but then things can get pretty confusing because sometimes you'll say proxy meaning a forward proxy and other times you'll refer to a reverse proxy as a proxy.

- ***Forward Proxy***
>- A forward proxy is a server that sits in between a client or a set of clients and another server or a set of other servers.
>- But more specifically a forward proxy is a **server that acts on behalf of the client or clients**.
>- You can almost think of the forward proxy as being on the client's team or on the client side of an interaction between a client and a server.
>- In practice, what this means is that if a client wants to communicate with a server, assuming the forward proxy has been configured correctly by the client, when the client is gonna issue a **request to the server, instead of going directly to the server, it's first gonna go to the proxy**, to the forward proxy, **which then is gonna forward the request to the server**.
>- So you can think of it as, the client does a request that's meant to go to the server, but first goes to the forward proxy.
>- It's almost like the client is saying, _"hey forward proxy, communicate with the server on my behalf please."_
>- And then the forward proxy will forward the request to the server.
>- Then the server gets the request, but the server gets it from the forward proxy.
>- The **server doesn't get the request directly from the client**.
>- So **when the server responds, it's gonna give its response to the proxy**, and the forward proxy is gonna give the response to the client.

> **A forward proxy can serve as a way to hide the identity of a client that's requesting something from a server.**

>- Because when the client issues the request that goes to the forward proxy, the forward proxy then forwards the request to the server, but the source IP address that's gonna be in this request that gets sent to the server from the forward proxy, is going to be the IP Address of the forward proxy.
>- In other words, the source IP address from the initial request, from the client can (in some cases) get removed and replaced by forward proxy's IP Address in this new request.
>- Because there are **some types of forward proxies** that might still **make this source IP address retrievable or visible** in some way to the server, but typically this original source IP address is not gonna be visible.

>- And so by the way, if you're familiar with VPNs, this is basically how VPNs work in a simplified way.
>- You have a forward proxy that sits in between you, the client and servers and the forward proxy or the VPN is gonna basically hide your identity.
>- And by the way this means that a client might be able to access restricted servers that it's otherwise not supposed to access because the forward proxy might hide who this client really is.
>- So this is how you might be able to access websites that are unavailable in your country, for instance, or that are restricted by your organization using a forward proxy.
>- So that's a forward proxy.

- ***Reverse Proxy***
>- Reverse proxies are a little bit trickier.
>- Whereas forward proxies act on behalf of clients in an interaction between a client and a server, **reverse proxies act on behalf of a server** in an interaction between a client and a server.
>- So the best way to think about it here, is that if a client wants to interact with a server, so the client wants to send a request to the server, if the reverse proxy has been configured properly by the server or by the entity that owns the server, then when the client is gonna issue a request to the server, the request is actually gonna go to the reverse proxy.
>- The **client won't know** that its **request is going to a reverse proxy**.
>- The client will think that it's just sending a request to the destination server, but it'll actually be going to the reverse proxy.
>- The client is gonna issue a request to the server, but if the reverse proxy has been configured properly, the request is actually gonna go to the reverse proxy, then the reverse proxy is going to forward the request to the server then the server is gonna return a response to the reverse proxy and finally the reverse proxy is gonna return the response to the client.
>- But so the key thing here is that the client thinks that it's interacting with the server.
>- In other words, to the client, there are no two entities (reverse proxy and server).
>- There's only one entity, they're one and the same and the client happens to think that that entity is the reverse proxy.

>- **For example**, what happens behind the scenes when you type [algoexpert.io](www.algoexpert.io) in your browser or [google.com](www.google.com) in your browser, and the browser makes a DNS query to get the IP address of [algoexpert.io](www.algoexpert.io) or of [google.com](www.google.com), if algoexpert or google use a reverse proxy and have it configured correctly, what's gonna happen is the DNS query is gonna return the IP address of the reverse proxy and not the one of the actual server.

>- So **this is really the opposite of forward proxy**.
>- In forward proxy, it's the server that has no idea that the client and the forward proxy are kind of one and the same, whereas with the reverse proxy, it's the client that has no idea that the reverse proxy and the server are effectively one and the same.

>- Now reverse proxies are really useful.
>- They're really useful because you can do a lot with them.
>- So when you're gonna be designing systems, especially complex systems, reverse proxies are definitely gonna be a tool that you're gonna want to have in your tool belt.

>- For instance, you might configure your reverse proxy such that it can filter out requests that you want to ignore.
>- Maybe for your system you don't want your servers to ever deal with certain kinds of requests so you can have your reverse proxy, kind of filter them out.
>- You can maybe **have your reverse proxy take care of logging** for your system.
>- If you wanna log stuff, if you wanna gather metrics, maybe your reverse proxy can do that.
>- If you wanna cache stuff, **maybe you wanna cache certain things like HTML pages**.
>- You might be able to do that at the reverse proxy layer and that way your server doesn't get bothered too much.

>- Perhaps **one of the best use cases** of a reverse proxy is using a reverse proxy as a **load balancer**.
>- In a sentence, a load balancer is something like a server that is gonna effectively distribute or that can distribute load, like request load between a bunch of servers.

>- So for instance, you can imagine that if you're designing a very complex system, you might have more than one server, you might have a bunch of servers, right?
>- You're gonna have a bunch of servers in your application and you can have your reverse proxy serve as a load balancer, that's gonna basically decide to what servers, all of these incoming requests from clients, has to be distributed across the servers following a specific pattern.
>- This might also have security ramifications.
>- For instance, imagine you had a client that was a malicious client that wanted to bring down a server by maybe issuing a ton of requests to a given server.
>- Well maybe your reverse proxy can act as a shield for that because it will distribute, again as a load balancer, it will distribute the requests maybe evenly amongst the various servers such that no single server gets all of the requests and gets taken down by this malicious client.
>- This is a simple example. But there are a lot of use cases for reverse proxies.

---

### 10. Load Balancers
> Relentlessly distributing network requests across multiple servers, these digital traffic cops act as watchful guardians for your system, ensuring that it operates at peak performance day and night.

#### 4 Key Terms
- ***Load Balancer***
> A type of **reverse proxy** that distributes traffic across servers. Load balancers can be found in many parts of a system, from the DNS layer all the way to the database layer.

- ***Server-Selection Strategy***
> How a **load balancer** chooses servers when distributing traffic amongst multiple servers. Commonly used strategies include round-robin, random selection, performance-based selection (choosing the server with the best performance metrics, like the fastest response time or the least amount of traffic), and IP-based routing.

- ***Hot Spot***
> When distributing a workload across a set of servers, that workload might be spread unevenly. This can happen if your **sharding key** or your **hashing function** are suboptimal, or if your workload is naturally skewed: some servers will receive a lot more traffic than others, thus creating a "hot spot".

- ***Nginx***
>- Pronounced "engine X", not "N jinx". Njinx is a very popular webserver that's often used as a **reverse proxy** and **load balancer**.
>- Learn more [https://www.nginx.com/](https://www.nginx.com/)

---

#### Understanding Load Balancers
>- Load Balancers are used in almost any system that you can imagine, you'll likely be using them in most, if not all your systems design interviews, and so it's very important that you know what they are and that you understand how they work.
>- Perhaps the best way to understand what a load balancer is to look at a very simple use case for a load balancer.

>- **For example**, let's assume there's a client and a server. The client issues requests and the server responds to the client.
>- Imagine what would happen if our system became a little bit bigger?
>- In other words, imagine instead of having one client issuing a request to our server, we had multiple clients, so maybe 2, 3 or 4 clients, all of them issuing requests to this server.
>- And you could imagine that one of our clients might be issuing more than one request, one of our clients might be issuing a lot of requests.
>- Our single server has limited resources. Our system has limited throughput.
>- Our single server can only handle a limited amount of requests in a given amount of time.
>- So what that means is that the more requests are being sent to the server, either from many clients or even just all from a single client, the more requests are being sent to our server, the more likely our server is to become overloaded, to receive more requests than it can handle.
>- And that might lead to a failure in our system or maybe it'll just make our system very slow.

>- So how do we handle this?
>- Well, the simple answer is, we scale our system.
>- And we have a couple of ways of doing this.

>- The **first way** is to vertically scale our system, meaning to increase the power of our server.
>- But as you can imagine, that's also going to be limited, there's only so much that we can do to increase the power or the performance of a single server of a single machine.

>- So then there's our **second option**, which is to horizontally scale our system, meaning to add more machines, to add more servers to our system.
>- And as you can imagine, horizontally scaling our system seems like a pretty obvious solution because if we have, let's say, 4 servers, we can now handle all of the requests from our clients in a balanced way.
>- And assuming that our servers have the same resources, have the same power, our system will be able to handle four times the load that it was previously able to handle with only one server.
>- But of course, this is assuming that all of our clients are going to be issuing requests to our servers in a balanced way.

>- But this begs the question, how did our clients know to issue their requests or rather to direct their requests to the servers in a balanced way?
>- How come none of the clients issued their requests to the same server leading to the same problem that we had before?

> **And this is of course where load balancers come into play.**

>- A load balancer is going to be a server that sits in between a set of clients and a set of servers and that basically has the job of, as its name suggests, balancing workloads across resources.
>- So in this case, **balancing or rerouting traffic from clients**, meaning requests, to these servers in a balanced way.
>- Because what would happen in this system with the load balancer is that our clients would be issuing requests, that would go to the load balancer.
>- And then the load balancers' job would be to redirect these requests in a balanced way or in some preconfigured way.
>- The **traffic is evenly distributed** across the servers.
>- And now, we have achieved our goal of horizontally scaling our system as it grew.

>- So load balancer is really useful because not only does it prevent resources like a single server or even multiple servers from getting overloaded, but it also makes your overall system have a better throughput.
>- if you have multiple servers that aren't being overloaded, then the throughput of your system is going to go up, your system might naturally get better latencies because your servers are going to be able to respond to requests faster because they won't be clogged or bogged down.
>- And you might make better use of your resources, because as you could imagine, if you are adding servers as you're horizontally scaling your system, the load balancer is going to know to make use of these new resources by distributing traffic to these new resources.
>- And so you'll be able to make use of them and perhaps alleviate the load to these other servers.

>- And by the way, you can think of load balancers as types of **reverse proxies** most of the time because load balancers sit between clients and servers, and they typically act on behalf of these servers, which is exactly what a reverse proxy does.

>- Load balancing can happen at a lot of different places in the system.
>- For instance, you can have a load balancer between the clients and servers, another one between the servers and databases or when dealing with a website, you might even have load balancing at the DNS layer.

>- Well, it turns out that there's something called **DNS Round Robin**, which is basically a type of load balancing that happens at the DNS layer, where a single domain name gets multiple IP addresses.
>- And when a DNS query is made to get back IP address of that domain name, the multiple IP addresses that are associated with that domain name are going to be returned in a load balanced way.

> ***How does this load balancer actually distribute this load***
>- Does it follow a special algorithm?
>- Does it do so randomly?
>- It is important, however, to note that there are different types of load balancers namely, there are some load balancers that are **software load balancers** and there are others that are **hardware load balancers**.
>- They are different.
>- **Hardware load balancers** are literally **physical machines** that are dedicated to load balancing.
>- The main difference between hardware load balancers and software load balancers is that you can **do more with software load balancers**, you have **more power over customization** and **scaling** with software load balancers.
>- With hardware load balancers, you're **limited to the hardware** that you're given. And hardware is often expensive.

> **We will look at software load balancers and the techniques that software load balancers use to distribute traffic to servers.**
>- So the first thing that you might be wondering is, how does a load balancer even know that it has servers to distribute traffic to?
>- And this is where basically, the people who are in charge of the system can **configure the load balancer and the servers** to know about each other.
>- You can make it such that when you add a new server or when you remove an old server, it registers itself with the load balancer or perhaps it deregisters itself with a load balancer so that the load balancer knows of its existence.

> **As for how load balancers actually select servers to send traffic to, there are a lot of different ways that they can do that.**
>- The **first one** that you might imagine is literally **pure random redirection**.
>- If you wanted to, you could configure your load balancer such that it would redirect traffic to all of your servers, following a purely random order.
>- Now, this might be fine. But as you can imagine, it could cause problems.
>- It could be possible that one server would by chance get overloaded.

>- So **another way** that load balancers often select servers is following a **Round Robin approach**.
>- So Round Robin is basically a method that goes through all of your servers in one order.
>- And so as you can imagine, that's pretty nice because you guarantee that you will be evenly distributing traffic across your servers.

>- A **slightly more complex type of Round Robin strategy** that you can have your load balancer follow is what's called a **Weighted Round Robin**, where you basically place weights on specific servers, meaning you would still follow the order of going to the first one first, then the second one, then the third one.
>- But you might put a weight on, let's say, the second server, which would mean that when your load balancer is redirecting traffic to your second server, it's going to redirect a couple more requests, a little bit more traffic than it redirects to the other servers.
>- And you could imagine that you might want to do that if, let's say, one of your servers is more powerful than the others.
>- And so you could have your load balancer follow a weighted Round Robin server selection strategy, where it would place more weight on this bigger server.

>- **Another way** for a load balancer to select servers is **based on performance or based on load**.
>- This strategy is a little bit more involved.
>- Basically, your load balancer performs health checks on your servers to know how much traffic a server is handling at any given time, how long a server is taking to respond to traffic, how many resources a server is using, and based on that, it'll redirect traffic accordingly.
>- So this can be a pretty good way for a load balancer to distribute traffic, depending on your use case.

>- **Another very common server selection strategy is an IP-based server selection strategy**, where basically, when your load balancer gets requests from clients, it's going to hash the IP address of the clients, and depending on the value of the hash, it will redirect the traffic accordingly.
>- IP-based load balancing can be really useful if you've got for instance, caching going on in your servers.
>- You could imagine that within your system you're caching the results of requests in your servers, it would be very helpful to have requests from a specific client always be redirected to the server in which the response of that particular client's request has been cached.
>- And that can be accomplished through this IP-based load balancing.
>- **IP-based load balancing can help you maximize cache hits**.

>- **One final method** of server selection for load balancers that can be very useful is a **path-based server selection strategy**.
>- With this strategy, a load balancer basically distributes requests to servers according to the path of the requests.
>- AlgoExpert uses this and they distribute some requests to different servers according to their path.
>- So basically, what this means is that all requests related to running code on AlgoExpert are going to be redirected to a specific server or a specific set of servers.
>- All requests related to payments on AlgoExpert, meaning purchasing the product are going to be redirected to another server or to another set of servers.
>- And this can be really useful because what it means is that if AlgoExpert ever wants to deploy a big change to their servers, like for instance, imagine that AlgoExpert wants to deploy a big change to their code execution engine, this deployment would only affect the servers handling the code execution engine requests, and all of the requests that are related to payments on AlgoExpert would still get routed to their own specific set of servers.
>- So if their code execution servers start dying for whatever reason, all the other services on the platform are unaffected.

> **So, there are a lot of different server selection strategies that your load balancers can have.**
>- And when you're going to be designing systems, you're going to want to **pick server selection strategies according to your use case**.
>- And the interesting thing about all of this is that when you're designing a system, it might actually **make sense to have multiple load balancers at different parts of the system that use different server selection strategies**.
>- And you're likely to **even have multiple load balancers at the same part of a system** because as you might be wondering, what happens if a load balancer starts to get overloaded?
>- Well, this is where you could have a second load balancer or even a third load balancer.
>- These load balancers could communicate between each other, and depending on that, reroute traffic accordingly.

> **Ultimately, load balancers are very simple, but they're extremely important.**
>- They are critical to large scale systems.
>- You will very likely, if not certainly, be using them in your systems design interviews.

---

### 11. Hashing
> Hashing? Like from hash tables? Should be simple enough, right?
> The good news is that, yes, hashing like from hash tables.
> The bad news is that, no, not simple enough.

#### 1 Prerequisite
- ***Hashing Function***
> A function that takes in a specific data type (such as a string or an identifier) and outputs a number. Different inputs may have same output. But a good hashing function attempts to minimize those **hashing collisions** (which is equivalent to maximizing uniformity).

#### 3 Key Terms
- ***Consistent Hashing***
> A type of hashing that minimizes the number of keys that need to be remapped when a hash table gets resized. It's often used by load balancers to distribute traffic to servers; it minimizes the number of requests that get forwarded to different servers when new servers are added or when existing servers are brought down.

- ***Rendezvous Hashing***
> A type of hashing also coined **highest random weight** hashing. Allows for minimal re-distribution of mappings when a server goes down.

- ***SHA***
> Short for "_**S**ecure **H**ash **A**lgorithms_", the SHA is a collection of cryptographic hash functions used in the industry. These days, SHA-3 is a popular choice to use in a system.

---

#### Understanding Hashing
>- Hashing is an action that you can perform to transform an arbitrary piece of data into a fixed size value, typically an integer value.
>- In the context of systems design interview, that arbitrary piece of data can be an IP address, a username, an HTTP request, anything that can be hashed or transformed into an integer value.

#### Where exactly does hashing come into play in a system?
>- Well for that, we can look at a pretty simple example.
>- We've got a fairly simple system consisting of clients, 4 clients in this case C1, C2, C3, C4.
>- These clients are going to be speaking with servers, four servers, A, B, C, and D.
>- But there's gonna be a load balancer in the middle.
>- So when the clients are gonna issue requests, these requests are first gonna go to the load balancer which is then gonna have to reroute them to the four servers.
>- When a load balancer has to redirect or reroute a request from a client to a server, it has to have some sort of server selection strategy (such as ramdom selection of servers, round robin approach etc.) to pick what server to reroute that request to.
>- And while a lot of these server selection strategies are fine at face value, they can introduce some problems depending on your system.

>- Let's assume, requests that are computationally expensive are gonna hit the servers and the servers have to perform very complex operations that take a long time to complete and so these requests are just so **expensive**.
>- One way to deal with these kinds of requests in a system is to use Caching.
>- So one way to implement caching here would be to have every server store an in-memory cache where every request that goes through a server, the server first checks if that request's response has been cached.
>- If it hasn't been, then it actually performs the operations and gets the response.
>- But if it has been cached, then it skips the operations that it would otherwise have to do and then immediately returns the cache response.
>- That would be a pretty reasonable way to design your system if you knew that these requests were gonna be very computationally expensive.
>- But this is where if your load balancer is selecting servers to reroute requests, following a round robin or a random strategy, this is where you're gonna have problems.
>- If you've designed your system in such a way that it relies heavily on in-memory caches in its servers, but your load balancer is rerouting requests from clients following a server selection strategy that doesn't guarantee that requests from a single client or the same requests will be rerouted to the same server every time, then your in-memory caching system is gonna fall apart and it's not gonna be as useful as it could be otherwise.
>- Basically, you're gonna miss a bunch of cache hits when your requests get routed to a server that doesn't have the responses cached.

#### And this is where hashing comes into play.

>- With hashing, what we can do is we can hash the requests that come in to the load balancer and then based on the hash, we can bucket the requests according to the position of the servers.
>- And then once we've hashed them, we can bucket the requests in the servers by performing a tiny bit of business logic.
>- For the sake of simplicity what we're gonna do here is we're just gonna hash the names of our clients.
>- We're gonna say that our goal is basically to get every client to have all of its requests rerouted to the same server so we're gonna be hashing the client's names themselves.
>- So we're gonna be hashing C1, C2, C3, C4.
>- And for the sake of this example, let's assume that we've got a hashing function that's been given to us and that when we pass C1, C2, C3, C4 through that hashing function, we get the following results.
>- We get 11 for C1, we get 12 for C2, we get 13 for C3 and we get 14 for C4.
>- Because remember that a hashing function basically transforms your arbitrary pieces of data into some fixed size value, typically an integer value.

#### So now what do we do with these four integer values?
>- Well the simplest thing that we can do, and this is really the simplest hashing strategy in the context of systems design interviews, is to ***mod these hashes here by the number of servers*** that we have.
>- So we're gonna mod all of these hashes by the number of servers, four servers, and this is gonna give us C1 -> 11%4 -> 3, C2 -> 12%4 -> 0 and so on.
>- So, C1 is associated with Server number 3 and so on.
>- And one important thing here is that, when you're dealing with a hashing function, it's important that the hashing function have what's known as uniformity.
>- You see how our clients got kind of evenly distributed amongst our four servers.
>- That didn't necessarily happen by chance.
>- But a really good hashing function would be able to do that as well, it would give you that sort of uniformity.
>- That's not to say that you might not have two clients mapping to the same server, you certainly could. Imagine you had more than four or eight or 12 clients.

>- But the point is, a good hashing function would still evenly distribute your data values.
>- That's just something to keep in mind when you're dealing with hashing.
>- And **in practice, you typically never write your own hashing function**.
>- **You use a pre-made industry-grade hashing function or hashing algorithm**.
>- A few popular examples are the MD5 hashing algorithm or the SHA-1 hashing algorithm, the Bcrypt hashing function, and you can trust that these hashing functions have that uniformity about them.

>- So now we will be maximizing our chance of getting cache hits for a client's requests.
>- So we fixed the problem that we described before where we were gonna miss our cache hits because of the server selection strategy of our load balancer which would make all of our clients' requests potentially hit different servers every time.

>- But of course, as you might expect, we have another problem now.
>- As you see we're dealing with a large-scale distributed system and when you have such a system, a lot of things can happen.
>- For instance, your servers can die.
>- We could very easily have server A fail on us and completely die.
>- Similarly, our system could be experiencing a ton of traffic and we might need to add servers to our system.
>- So maybe our server A doesn't die, but maybe we need to add a new server to our system, server E to handle some new incoming traffic.
>- What do we do if we need to add a fifth server which is not an unreasonable thing to expect if we're dealing with a large-scale system.
>- What do we do if we need to add server E?
>- We can't continue to mod all of our hashes by four because we no longer have four servers. We have five servers.
>- If we keep modding our hashes for our clients by four, then all of our requests are always only gonna go to servers A, B, C, and D. They're never gonna go to E.
>- And before if server A had died and we hadn't added E, then we wouldn't have been able to continue to mod by four 'cause requests would've continued to get routed to A and A would've been dead and so our users would not have been happy.

>- So the point is, if a server dies or here, if we add a new server, we have to change some logic here.
>- Namely, we have to mod our hashes by the new number of servers.
>- In this case, the new number of servers is five.
>- Okay, so let's mod all these hashes by five.
>- C1 -> 11%5 -> 1 and so on.
>- So as you can see, when we mod our hashes by 5 instead of 4, we get completely different results for the servers that our clients are going to be rerouted to.
>- And what that means is that we're gonna once again face our problem of missing a bunch of cache hits 'cause if C1 which was previously going to server D now goes to server B, all of the value that we had from our in-memory cache at server D is lost 'cause server B has never cached stuff related to client 1.
>- And the same thing applies to all of the other servers and all of the other clients and this is really, really bad when you've got a huge system.

>- So all this to say our very simple hashing strategy of hashing our clients or usernames or requests or IP addresses, whatever, and then modding the hashes by the number of servers to figure out what server to reroute stuff to just doesn't work because the second that one of your servers dies, or the second that you have to add another server, everything becomes a mess and all of your in-memory caches that you may have had in your system are no longer useful.

#### Okay, so how do we solve this problem?
>- What do we do when we have to add a server or when we have to remove a server?
>- Well, this is where consistent hashing and rendezvous hashing come into play.

> ***These two slightly more complicated hashing strategies basically fix this problem and we're gonna cover them now.***

>- For consistent hashing, we're gonna imagine that instead of having our servers A, B, C, D, E.
>- We're gonna actually put them on a circle.
>- This circle is not an actual thing, it's more a concept that helps us visualize this consistent hashing strategy better.
>- So imagine that you had this big circle here and that you've placed your servers on the circle in a sort of evenly distributed way.
>- How exactly are we placing these servers on the circle?
>- Well you can imagine that this circle basically represents a bunch of numbers, so it might start at the top with zero and then it would increment as you move along the circle in a clockwise way, all the way until you reach the top again, at which point maybe you would reach the number 360 if you wanna make this seem like degree angles or maybe it would be some other number.
>- The point is, this circle can be represented as a bunch of back to back numbers.
>- But conceptually, it looks like a circle that loops around and the way that you place these servers here on the circle is by putting them through a hashing function.
>- You could imagine that you could put the servers, let's say the server names in a hashing function. You get a value and depending on the value, you position them on the circle.
>- If you're hashing function is a good hashing function that has that uniformity about it, then the servers will be sort of evenly distributed.

>- Okay, so what comes next?
>- Well you do the exact same thing with your clients.
>- So let's take our four clients that we had in the previous example.
>- Our four clients are gonna go through a hashing function and again here this might be the client's IP addresses, maybe we're talking about actual HTTP requests, maybe we're talking about the client's usernames, for the sake of the example, it doesn't really matter.
>- We're kind of using these terms loosely, but you put them through the hashing function and then you position them on the circle.
>- So now you've positioned your servers on the circle, and you've positioned your clients on the circle.
>- How do you determine where requests or where clients are going to be routed to?
>- Well, you go to each client and from each client, you move clockwise in a clockwise direction and here of course, you could actually move in a counter-clockwise direction if you wanted to, it's really a matter of preferences.
>- You just have to decide how you wanna implement this consistent hashing strategy.
>- Let's go with clockwise for the sake of this example.
>- So you move in a clockwise direction from each client, and the first server that you encounter is gonna be the server that your load balancer is gonna reroute this client to, or this client's requests to.
>- So C1 might be directed to Server A and so on.
>- So as you can see, this is kind of uniformly distributed because we used these hashing functions to position our servers and our clients.

>- But what does this accomplish?
>- Well let's see what happens if one of our servers dies.
>- What if server C dies? Remember in the previous example with a simple hashing strategy, like we said, if a server died, we'd have to redo all of our calculations.
>- We would no longer be able to mod by let's say four if one of our servers died, we would have to mod by three.
>- Here, if one of our servers dies, let's say server C, we're gonna go back to our clients, move in a clockwise direction, and find the closest servers.

>- What happens if we add a new server?
>- We go through our clients, move clockwise.
>- So as you can see with this system, with this system of putting the servers and the clients on a circle and moving in a clockwise direction, what we accomplish is that if we ever add or remove a server, we actually still maintain most of the previous mappings or associations between clients and servers.
>- Only a few of them change.

>- This is why consistent hashing is so powerful because basically, it maintains some level of consistency between hashes and their target buckets.
>- And so in the context of systems design interviews, it maintains some good level of consistency in the mappings between the clients or the requests or the IP addresses, whatever you use and the servers or whatever else you're mapping them to.

>- What's also cool about consistent hashing that you can with this circle concept, is let's say you wanna even more evenly distribute your traffic.
>- Because here you might argue that hey, maybe a lot of your clients or a lot of your requests are gonna somehow get hashed in a section of the circle where one of the servers isn't present.
>- Maybe most of your clients and requests are gonna appear on the right side of the circle.
>- So what you can do is you can pass all of your servers through multiple hashing functions and then place all of the hashes that you get for your servers on the circle and so basically each server will have multiple places that are associated with it.
>- So before this, it was like.. Imagine in a circle, clockwise, the servers and clients are mapped as follows:
>- C1, E, C4, A, C3, B, C2, C and so on.
>- Now the circle looks like..
>- C1, E, C4, A, C3, A, C2, E and so on.
>- So, a server, for example, A can be placed at multiple places in the circle.

>- What this also allows you to do is let's say that one of your servers is more powerful than the others.
>- Imagine at the very beginning of the life of your system, you only had one server, server A, and when your system started to grow, you decided to scale it vertically by making your main server A more and more powerful.
>- Eventually, you decided to scale horizontally by adding servers like B, C, D, and E.
>- But they were all weaker, not as powerful at server A so now you're faced with a situation where you wanna evenly distribute your traffic amongst your servers, but you want A to get a little bit more of the load because it's a more powerful server and you still wanna use this consistent hashing strategy.
>- Well what you can do is you can pass server A through more hashing functions than all the other servers and so what ends up happening is server A will have more locations on the circle.
>- Servers B, C, D, and E might have two locations, But then you might give A let's say five locations.
>- So basically now, there's just a higher likelihood that any given client or request is gonna bump into A when you move clockwise from it.
>- ***So this is consistent hashing and it's very powerful***.

> ***Now let's look at another kind of complicated hashing strategy, or at least more complicated than the arguably naive one that we used at the very beginning.***

>- This one is rendezvous hashing.
>- So imagine that you've got a bunch of usernames (Username 0, 1, 2, 3, 4, 5, 6, 7, 8, 9) and servers (Server 0, 1, 2, 3, 4, 5).
>- So what the rendezvous hashing strategy is gonna do is for every username, it's going to calculate a score or rather a ranking of the servers or the destinations, whatever the destinations may be in your use case.
>- So in this case, it's gonna say hey, for username0, I'm gonna rank these six servers using some formula or some piece of logic, and I'm gonna pick the highest ranking server.
>- Then for username1, I'm gonna do the exact same thing and so on.
>- So let's say that username0 finds server0 as the highest ranking server for itself.
>- That's the server that it's going to be associated with.
>- And so when you remove a server, you could imagine that if username0 had server0 as its highest ranking server, removing server5 isn't gonna do anything and username0 is still gonna map to server0.
>- On the other hand, let's say that username2 mapped to server5 and then you remove server5, then that means that you will naturally have to change the mapping of username2 and you will just take the second highest ranking server which would be whatever other server, it doesn't matter, and that would change.
>- ***So that's how rendezvous hashing works in a nutshell.***
>- Basically calculate scores for your servers or for your destination buckets. Pick the highest one, and that's the thing that your value, in this case your username is gonna be associated with.
>- And so as you can see, just like with consistent hashing, we maintain some consistency in these mappings, in these associations, and that is really useful in the context of systems design.
>- And I think that it's easy not to appreciate how useful it is when you don't work with a large-scale system.
>- Here, we're seeing kind of small examples so, it seems sort of trivial.
>- Imagine that you have a large-scale system.
>- Let's say an e-commerce website like Amazon and you're getting ready for Cyber Monday where you're expecting huge amounts of traffic and you're gonna be relying heavily on in-memory caching strategies, for instance.
>- Do you want your users to experience really high latencies because some of your servers are dying or if you have to add new servers and your hashing strategy is poor in making it such that you're missing a bunch of cache hits?
>- No, you don't want that, 'cause that can lead to a ton of lost business, you could be talking about millions of dollars on the line.
>- The point is, when you've got a large-scale system, this becomes really really important.

> ***So when you walk into your systems design interviews, make sure to have these hashing strategies in your tool belt to be aware of when you might need to use something like consistent hashing or rendezvous hashing.***

>- Both of those are fairly interchangeable, they both accomplish kind of the same thing.
>- But the naive hashing strategy, the one where you just mod the hashes by the number of servers that you have for instance, that one is certainly not as good.
>- And if your system is gonna be relying on something like in-memory caching, you're definitely gonna wanna be able to bring up these hashing strategies.

---

### 12. Relational Databases
> ***Tables*** and ***ACID***.

> No, we're not describing a drug lord's desk, but rather referring to key properties of relational databases. There's a lot of material to cover here, so kick back, and get ready to store tons of knowledge in the biggest database of them all: your brain.

#### 10 Key Terms

- ***Relational Database***
> A type of structured database in which data is stored following a tabular format; often supports powerful querying using SQL.

- ***Non-Relational Database***
> In contrast with relational database (SQL database), a type of database that is free of imposed, tabular-like structure. Non-relational databases are often referred to as NoSQL databases.

- ***SQL***
> Structured Query Language. Relational databases can be used using a derivative of SQL such as PostgreSQL in the case of Postgres.

- ***SQL Database***
> Any database that supports SQL. This term is often used synonymously with "Relational Database", though in practice, not every relational database supports SQL.

- ***NoSQL Database***
> Any database that is not SQL-compatible is called NoSQL.

- ***ACID Transaction***
> A type of database transaction that has four important properties:

>- ***Atomicity:*** The operations that constitute the transaction will either all succeed or all fail. There is no in-between state.
>- ***Consistency:*** The transaction cannot bring the database to an invalid state. After the transaction is committed or rolled back, the rules for each record will still apply, and all future transactions will see the effect of the transaction. Also named ***Strong Consistency***.
>- ***Isolation:*** The execution of multiple transactions concurrently will have the same effect as if they had been executed sequentially.
>- ***Durability:*** Any commmitted transaction is written to non-volatile storage. It will not be undone by a crash, power loss, or network partition.

- ***Database Index***
> A special auxillary data structure that allows your database to perform certain queries much faster. Indexes can typically only exist to reference structured data, like data stored in relational databases. In practice, you create an index on one or multiple columns in your database to greatly speed up ***read*** queries that you run very often, with the downside of slightly longer ***writes*** to your database, since writes have to also take place in the relevant index.

- ***Strong Consistency***
> Strong Consistency usually refers to the consistency of ACID transactions, as opposed to ***Eventual Consistency***.

- ***Eventual Consistency***
> A consistency model which is unlike ***Strong Consistency***. In this model, reads might return a view of the system that is stale. An eventually consistent datastore will give guarantees that the state of the database will eventually reflect writes within a time period (could be 10 seconds, or minutes).

- ***Postgres***
> A relational database that uses a dialect of SQL called PostgreSQL. Provides ACID transactions.

---

> It is difficult to make generalising statements about these databases. It's hard to categorize these databases into specific bucket.

> However there's one characteristic that we can use to actually categorize all of these databases specifically into two major categories.

> And that characteristic is the **structure that is imposed on the data** that you store in these databases.

> This is where relational databases come into play.

> It turns out that one of the **two major categories of databases**, if we are specifically looking at the structure imposed on the data stored in these databases, is relational databases.

> So we have **relational databases vs non-relational databases**.

-  ***So what is a relational database ?***

>- A relational database is a type of database that imposes on the data stored in it, a **tabular-like structure**.

>- In other words, data stored in a relational database is gonna be stored in the form of tables.

>- So tables, which are also called as relations and relational databases, are these structures that store a bunch of data.

>- They typically **represent a specific entity**.

>- Rows in a relational databases are often referred to as records.

>- All the tables that are stored in a relational database are going to **have defined schemas, the specific rules or plans about how the data should be stored in them**.

>- And the systems designer or the person setting up these relational databases, is gonna be the one defining these schemas.  

-  ***Non-relational database ?***

> In contrast with the relational databases, non-relational databases are databases that don't impose this tabular-like structure on the data stored in them.

> While non-relational databases do sometimes impose some type of structure on the data stored in them, it's typically not gonna be in the form of tables and it's typically gonna be a lot more flexible and a lot less rigorous.

> Prehaps one of the **most important aspects of relational databases** is that most relational databases out there, there are always exceptions, but **most of them support SQL**.

>- SQL, which stands for **S**tructured **Q**uery **L**anguage, SQL is effectively a programming/database/querying language.

>- But SQL is a very powerful language that is **used to perform complex queries** in relational databases.

>- A SQL Database must use what are known as **ACID** transactions.

>  - **A** - Atomicity
>  - **C** - Consistency
>  - **I** - Isolation
>  - **D** - Durability

-  ***Database Index***

>- Imagine you have a table (Payments table in this case) in a relational database.
>- And imagine that you want to look for the name of the customer who paid the largest amount of money.
>- To do that, you naturally gonna have to look through the entire database to find the largest amount.
>- This is a **linear time operation O(N)**.
>- And if you are dealing with huge tables that have millions of rows, then this is gonna be really slow, especially if you need to perform these types of operations over and over and over again.
>- And this is where a **database index comes into play**.

>- Database indexes are very complicated.
>- There're a lot of types of database indexes out there, different ways that they can be implemented under the hood.
>- There're bitmap indexes, reverse indexes, dense indexes etc.
>- **An example** for database index: An auxillary data structure, almost like an additional table, that stored the amounts of all of the payments, that stored the amounts in sorted order.
>- And they would all point to the relavent records in the table.
>- You can think of a database index as a table of contents.

>- So database indexes are a good thing to keep in mind when designing the database part of a system.
>- If you go with a relational database and you happen to know that you're gonna be searching that database a lot, you may want to have certain database indexes for some of your tables.

>- **The trade-off** to keep in mind when thinking about adding a database index is that having a database index, because it's effectively an auxillary data structure, is gonna take up more space.
>- And it's gonna mean that whenever you write to the database that has a database index, you're also gonna have to write in the database index.
>- So write operations are gonna be a little bit slower and taking up more space, but read operations might be a lot faster.

---

### 13. Key-Value Stores
> One of the most commonly used NoSQL paradigms today, the key-vaue store bases its data model on the associative array data type.

> The result ? A fast, flexible storage machine that resembles a hash table. That's right folks, our favorite frendly neighbourhood data structure strikes again!

#### 4 Key Terms
-  ***Key-Value Store***
> A Key-Value Store is a flexible NoSQL database that's often used for caching and dynamic configuration. Popular options include DynamoDB, Etcd, Redis and ZooKeeper.

- ***Etcd***
>- Etcd is a strongly consistent and highly available key-value store often used to implement leader election in a system.
>- Learn more: [https://etcd.io/](https://etcd.io/)

- ***Redis***
>- An in-memory key-value store. Does offer some persistent storage options but is typically used as a really fast, best-effort caching solution. Redis is also often used to implement **rate limiting**.
>- Learn more: [https://redis.io/](https://redis.io/)

- ***ZooKeeper***
>- ZooKeeper is a strongly consistent, highly available key-value store. It's often used to store important configuration or to perform leader election.
>- Learn more: [https://zookeeper.apache.org/](https://zookeeper.apache.org/)

---

>- The structure of relational databases is often very useful because it typically comes with very powerful querying capabilities.
>- But sometimes, that same structure is actually more cumbursome than useful.
>- And in those cases, a non-relational database, a **NoSQL database** is preferred, **a database, that doesn't come with any structure**.

>- And it turns out that one of the **most popular** types of non-relational databases out there is the **key-value store**.
>- The key-value store, as it's name implies, is a type of database that allowes you to store key-value pairs.
>- And these values are typically stored as strings, but some key-value stores do actually come with specific typings, so that'll allow to store actual integers or actual arrays, all sorts of other values.  

>- Now, what's great about key-value stores, is that they are **incredibly flexible** and **incredibly simple**.
>- Flexible because they don't have the imposed structure and simple because there's arguably no simpler type of storage at least from a conceptual point of view than a key-value type of mapping.
>- And so this makes key-value stores, awesome candidates for databases in a system where there's no use for that imposed structure.
>- **Example:** *Caching*  

>- If you think about caching, it's actually something that lands itself perfectly to key-value stores, because when you implement caching, you're typically storing values like reponses to network requests.
>- You typically store these values somewhere and access them using a hash, using an IP address, a username.
>- The point is, you access them using some sort of key.
>- So conceptually, you're precisely using the key-value pair model.
>- And so key-value stores are often great databases to use for caching in a system.

>- **Another use case** that comes to mind is for **dynamic configuration**.
>- Sometimes the system might have special parameters, or constants that different parts of system can rely on.

>- Key-value stores have a lot of use cases.
>- And one other thing that makes them really nice is that because you are accessing values directly through keys, **you don't have to search through the database by sequentially going through every entry** or by doing some other fancy lookup.
>- You can just access values directly through keys and that makes them very fast.
>- So often by using a key-value store, you'll actually get **lowered latencies** and **increased throughput** in whatever part of your system uses a key-value store.  

>- One more important thing to mention about key-value stores is that they come in **various shapes and flavors**.
>- There are a lot of databases out there and naturally there are a lot of key-value stores out there.
>- Few examples are DynamoDB, Etcd, Redis, ZooKeeper etc., and **different key-value stores might behave differently**.  

>- For instance, **some key-value stores writes data to disk**. Meaning, the data that is stored is gonna persist even if key-value store goes down. 
>- Other key-value stores **might write data only to memory**. Redis is a very popular example for that. Redis is an in-memory key-value store.

>- So if those type of key-value stores crash, the data stored in them is lost.
> Now this is a **trade-off** for faster operations and depending on the use case, it might be totally acceptable.
>- Some key-value stores might give **strong consistency**, others might give only **eventual consistency**.

---

### 14. Specialized Storage Paradigms

#### 11 Key Terms
- ***Blob Storage***
> Widely used kind of storage, in small and large scale systems. They don't really count as databases per se, partially because they only allow the user to store and retrieve data based on the name of the blob. This is sort of like a key-value store but usually blob stores have different guarantees. They might be slower than KV stores but values can be megabytes large (or sometimes gigabytes large). Usually people use this to store things like **large binaries, database snapshots, or images** and other static assets that a website might have.

> Blob storage is rather complicated to have on premise, and only giant companies like Google and Amazon have infrastructure that supports it. So usually in the context of System Design interviews you can assume that you will be able to use **GCS** or **S3**. These are blob storage services hosted by Google and Amazon respectively, that cost money depending on how much storage you use and how often you store and retrieve blobs from that storage.

- ***Time Series Database***
> A **TSDB** is a special kind of database optimized for storing and
analyzing time-indexed data: data points that specifically occur at a given moment in time. Examples of TSDBs are InfluxDB, Prometheus, and Graphite.

- ***Graph Database***
> A type of database that stores data following the graph data model. Data entries in a graph database can have explicitly defined relationships, much
like nodes in a graph can have edges.

> Graph databases take advantage of their underlying graph structure to perform complex queries on deeply connected data very fast.

> Graph databases are thus often preferred to relational databases when dealing with systems where data points naturally form a graph and have multiple levels of relationships. For example, social networks.

- ***Cypher***
> A **graph query language** that was originally developed for the Neo4j
graph database, but that has since been standardized to be used with other
graph databases in an effort to make it the "SQL for graphs."

> Cypher queries are often much simpler than their SQL counterparts. Example Cypher query to find data in **Neo4j**, a popular graph database:
```
MATCH (some_node:SomeLabel)-[:SOME_RELATIONSHIP]->(some_other_node:SomeLabel {some_property:'value'})
```

- ***Spatial Database***
> A type of database optimized for storing and querying spatial data like
locations on a map. Spatial databases rely on spatial indexes like **quadtrees** to quickly perform spatial queries like finding all locations in the vicinity of a region.

- ***Quadtree***
> A tree data structure most commonly used to index two-dimensional spatial
data. Each node in a quadtree has either zero children nodes (and is therefore a leaf node) or exactly four children nodes.

> Typically, quadtree nodes contain some form of spatial data. For example,
locations on a map with a maximum capacity of some specified number **n**. So long as nodes aren't at capacity, they remain leaf nodes; once they reach capacity, they're given four children nodes, and their data entries are split across the four children nodes.

> A quadtree lends itself well to storing spatial data because it can be
represented as a grid filled with rectangles that are recursively subdivided into four sub-rectangles, where each quadtree node is represented by a rectangle and each rectangle represents a spatial region. Assuming we're storing locations in the world, we can imagine a quadtree with a maximum node-capacity **n** as follows:
>	- The root node, which represents the entire world, is the outermost rectangle.
>	- If the entire world has more than **n** locations, the outermost rectangle is divided into four quadrants, each representing a region of the world.
> 	- So long as a region has more than **n** locations, its corresponding rectangle is subdivided into four quadrants (the corresponding node in the quadtree is given four children nodes).
>	- Regions that have fewer than **n** locations are undivided rectangles (leaf nodes).
>	- The parts of the grid that have many subdivided rectangles represent densely populated areas (like cities), while the parts of the grid that have few subdivided rectangles represent sparsely populated areas (like rural areas).

> Finding a given location in a perfect quadtree is an extremely fast operation that runs in **log<sub>4</sub>(x)** time (where x is the total number of locations), since quadtree nodes have four children nodes.

- ***Google Cloud Storage***
>- GCS is a blob storage service provided by Google.
>- Learn more: [https://cloud.google.com/storage](https://cloud.google.com/storage)

- ***S3***
>- S3 is a blob storage service provided by Amazon by **Amazon Web Services (AWS)**.
>- Learn more: [https://aws.amazon.com/s3/](https://aws.amazon.com/s3/)

- ***InfluxDB***
>- A popular open-source time series database.
>- Learn more: [https://www.influxdata.com/](https://www.influxdata.com/)

- ***Prometheus***
>- A popular open-source time series database, typically used for monitoring purposes.
>- Learn more: [https://prometheus.io/](https://prometheus.io/)

- ***Neo4j***
>- A popular graph database that consists of **nodes, relationships, properties,** and **labels**.
>- Learn more: [https://neo4j.com/](https://neo4j.com/)

---

- ***What is a blob store ?***
>- Well, a blob, first of all is an acronym, it stands for **binary large object**, but in the modern day, so to speak and in systems design interview, or in systems design context, when someone uses the word blob, they're really referring to just some **arbitary piece of unstructured data**.
>- An example for a blob is gonna be a video file or an image file, may be a large text file, or may be a large binary, meaning compiled code that's ready to be shipped out to production.

>- And so a blob store as it's name suggests, is a **storage solution for blobs**.
>- Because a blob isn't really the type of data that fits into for example a SQL database.
>- A **blob is unstructured data**.
>- It's not the type of data that makes sense to store in a tabular format.
>- And **oftentimes blobs are very large**.
>- And if you have multiple blobs, if you've got millions of blobs, and you've got really massive amounts of unstructured data.
>- And that is what a Blobstore specializes in doing.
>- A Blobstore specializes in storing massive amounts of unstructured data.
>- Blobstores are optimized for storing and retrieving massive amounts of unstructured data.
>- And this is actually a **pretty complicated problem to solve**.

>- So you will basically never or very rarely find yourself implementing your own Blobstore solution.
>- You will **almost always rely on some popular Blobstore solution** like S3 or GCS.

>- Also one last thing to note about Blobstores is that they **sort of behave like key-value stores** in the sense that usually when you're accessing a blob in a Blobstore, you're accessing it through some key, whether that's the blobs ID or the blobs name.
>- So that's kind of like a key-value store, but you shouldn't mistake or confuse Blobstores and key-value stores.
>- Because ultimately they are optimized for different functionalities or use cases.

- **Time Series Database**
>- This one is **a little bit less commonly encountered than the Blobstore**, mainly because you're less likely at least in the context of systems design interview, to encounter time series data than you are to encounter large unstructured data, which is why a blob store is necessary usually.
>- It's still worth being familiar with the time series databases, knowing that they exist, and being able to refer to a couple of technologies that you could use in the event that you needed a time series database.

>- Time series databases are **often used in logging and monitoring purposes**.
>- A time series database as its name suggests is a database that is specialized for storing time series data.
>- So when you've got large amounts of data that are all relevant to time, in other words, they are let's say maybe events that happen at a given time. Let's say every second or every millisecond.
>- When you've got that type of data and when you're gonna be likely to have to perform very time series like computations on this data, things like computing rolling averages, or computing local maximas and minimas or aggregating data in between two time periods.
>- When you've got that time type of data or that type of requirement or use case you're likely gonna use a time series database.

> So some of the very common use cases for time series databases are monitoring, if you're monitoring parts of your system, for example, you've got a bunch of events that all occur at a given timestamp. You might wanna use a time series database to store them.

> Or for example, if you're designing an IOT system, an internet of things system where you've got millions of devices that are constantly, sending telemetry data or capturing certain data in their environments, when you've got that type of system, a time series database is likely gonna be useful.

> If you're dealing with stock prices maybe that change every second or cryptocurrency prices, you might need a time series database.

> So here, two of the most popular time series databases out there are InfluxDB and Prometheus.

> **You don't need to be super well versed with time series databases. And so naturally you don't need to know too much about these technologies. Ideally you just wanna know that they exist. You wanna be able to refer to them if you need a time series database in your system, and you can say something like, *"Oh, for the monitoring part of our system, we can rely on InfluxDB"*.**

> So those are time series databases in a nutshell.

- **What is a Graph Database**
>- It serves as a nice **bridge between data structures & algorithms and systems design**, because it uses the graph data structure or relies on concept of a graph.

>- If you're storing a dataset where within the data, there are a lot of relationships, relationships between individual data points in the dataset.
>- A tabular format, might not make as much sense.

>- So a graph database is a database that is built on top of the graph data model.
>- So what that means is that in a graph database, the concept of a relationship between data points is a primary concept. It is something core to a graph database.

>- And so what that means for graph databases is that when you have graph like data, when you have data that lends itself really well to being stored in a graph, meaning data, where there a lot of relationships and here you can think of social networks like Facebook, where people have a lot of friends. And there are a lot of links between people and concepts on the website like pages and posts that are shared, etc. When you've got that type of dataset, a graph database allows you to rely on the natural data model which is the graph that this data set lends itself really well to, for all of your querying functionality and all of your storage functionality.
>- And so the most popular graph database out there is a database called Neo4j.

- **What is a Spatial Database**
>- A special database that is optimized for storing spatial data.
>- What is spatial data ? Anything that has to do with geometric space, but the canonical example in systems design or in the context of systems design interviews is gonna be locations on a map.
>- Let's say that you're storing hotels in the world or restaurants in a country. Maybe you're designing Google maps. You might very well, want to rely on a spatial database to store all of this data.

#### Now, how does a spatial database work exactly? 
>- If you wanna perform certain queries very fast, that rely on a particular column in a SQL table, You might wanna create a database index on that column.
>- And that works really well for standard data.
>- But when you're dealing with spatial data. So for example, let's say you're storing latitudes and longitudes.
>- And so you're relying on two different attributes and you might be performing spatial related queries, like finding all locations in the vicinity of a specific location or finding the distance between two locations or multiple locations.
>- A standard database index might not be as good, might not be optimized for this type of query or this type of computation.

>- And so spatial databases, what they do is they rely on **spatial indices**. So instead of having a classic database index, you have a spatial index.
>- And here there are a lot of different types of spatial indices out there.
>- One such index is Quadtree.

- **What is a Quadtree ?**
>- A lot of spatial indices are based on trees such as R-trees, K-D trees, M-trees etc.

>- Quadtree is fairly straightforward to understand conceptually and it's pretty common and it's just a really cool index.
>- Basically a quadtree is just like a binary tree except that every node has 4 children nodes instead of two.
>- Or specifically in a quadtree, every node has either zero children nodes and therefore is a leaf node, or it has exactly four children nodes.
>- A quadtree would have always four children nodes or no children nodes.

>- We can compare the quadtree to the tree data structure, but conceptually, it is actually in the form of grid format.
>- And then the nice thing about this quadtree and this grid format is that when you're performing spatial queries on this data, you can traverse through this quadtree, traverse through this grid very easily in log<sub>4</sub>(N) time.
>- And you can just find what you're looking for very, very fast.
>- So this quadtree is optimized for performing some of these spatial queries.
>- So this is what a quadtree is.
>- It's a very popular spatial index used by spatial databases.
>- Sometimes you might even find yourself implementing your own quadtree and maybe storing it in memory, depending on the system that you're designing.

>- Let's say you're designing a system where you really, really care about very fast latencies.
>- You're obviously dealing with a location based system or a system that relies on spatial data, and you don't wanna be querying your database all the time.
>- You might wanna just stop at your API servers. You might build your own quadtree and store in memory there.

>- In this day and age, a lot of databases, including even standard databases, like let's say Postgres are really, really smart, are really, really optimized for all sorts of queries and data types.
>- So it's possible that some databases like Postgres might even give you out of the box solutions for spatial data.

>- **So depending on the systems design interview and on your interviewer, you might be able to get away with just relying on a classic database.**
>- Even if you're relying on spatial data, it's all gonna depend on what your interviewer's looking for.
>- And it might warrant having a conversation with them where you say, *"Hey, here, we're relying on spatial data. I'm thinking that we could maybe use a specialized spatial database or even implement our own spatial index and memory. Or maybe we can just rely on out of the box optimizations that a database like Postgres might give us, what do you think, what are we looking for here?"*
>- And hopefully your interviewer would be able to guide you in the right direction for what they're looking for in their systems design interview.

---

### 15. Replication And Sharding
> A system's performance is often only as good as its database's; optimize the latter, and watch as the former improves in tandem!

#### 3 Key Terms

- ***Replication***
> The act of duplicating the data from one database server to others. This is sometimes used to increase the redundancy of your system and tolerate regional failures for instance. Other times you can use replication to move data closer to your clients, thus decreasing the latency of accessing specific data.

- ***Sharding***
> Sometimes called **data partitioning**, sharding is the act of splitting a database into two or more pieces called **shards** and is typically done to increase the throughput of your database. Popular sharding strategies include:
>	- Sharding based on a client's region
>	- Sharding based on the type of data being stored (e.g: user data gets stored in one shard, payments data gets stored in another shard)
>	- Sharding based on the hash of a column (only for structured data)

- ***Hot Spot***
> When distributing a workload across a set of servers, that workload might be spread unevenly. This can happen if your **sharding key** or your **hashing function** are suboptimal, or if your workload is naturally skewed: some servers will receive a lot more traffic than others, thus creating a "hot spot".

---

>- Because a database is so critical to a system, a system's performance is often very dependent on it's database's performance.
>- So, for example, if a system's database is unavailable, then the system itself will likely be unavailable.
>- If a system's database has high latency or low throughput, then the system itself will likely have high latency or low throughput.

>- So when we're designing a system and trying to make it performant, we have to make sure that the system's database is gonna be performant, otherwise the entire system is likely gonna fall apart.
>- This is where replication and sharding come into play.

#### Let's start with replication
>- Imagine that you've got a system and the system has got a database. We'll go with a single main database and that database goes down.
>- Well, suddenly you can't read data from the database, you can't write data to the database, your system is effectively down as well.

>- How would you remedy the situation, or rather, how would you prevent the situation from happening in the first place?
>- Well, you might do so by having a secondary database, a replica of the main database, and this is replication in a nutshell.
>- The idea behind replication is that you have a duplicate version of your main database, a replica of the main database. And in this example, you can think of this replica sort of like a standby of the main database.
>- The main database handles all of the reads and writes coming to it, but it also updates the replica such that the replica is effectively the same as the main database.
>- The idea is, the replica would take over if the main database fails.
>- So when the main database goes down, the replica takes over and now becomes the new main database.
>- And once the original main database comes back up, it gets updates by the replica, and then eventually they can swap roles again.

>- Now in order for this to work, your replica needs to always be exactly up to date with the main database.
>- So what that means is that whenever someone writes/udates to the main database, that update needs to also happen in the replica in a synchronous way.
>- If you wanna have your replica be able to take over when your main database fails, you need that replica to always be up to date with the main database, and so that means that whenever there's a write operation to your main database, that write operation needs to synchronously be done on the replica as well.
>- And for whatever reason, that right operation fails on the replica, there's an issue, a network partition, whatever, then the write operation should not complete on the main database.

>- In this scenario where you want your replica to be able to take over for your main database in the event of database failure, you never want the replica to be out of date with the main database.
>- And of course, this means that your write operations are gonna take a little bit longer, because they have to be done both on the main database and on the replica.

> So this was a fairly straightforward example of using replication to improve the availability of your database and of your system as a whole, but we can also use replication to improve our database's latency and in turn to improve our system's latency.

>- Let's look at an example for this.
>- Imagine that we were designing a system like LinkedIn, where people can write posts and other people can view those posts in their feed.
>- And imagine that we know that we're gonna have a lot of users, both in the US and in India.
>- What we might do is we might have two databases, one in the US, serving US users, and one in India, serving India users.
>- That way, US users and India users get very low latencies, because they're served the data from databases located in their regions.

>- Now what happens if I, a user located in the US, write a post on LinkedIn.
>- That post will be stored in the US database, and I'll experience very low latency when I actually post the post.
>- But then my post, which is stored in the US database, needs to be replicated in the India database, because you can imagine that I might have a lot of connections or followers on LinkedIn who are based in India, and so they're gonna need to see my post in their feed.
>- But because we're talking about a feed here where maybe we don't care about having someone's post instantaneously appear in other people's feeds, what we can do is we can have the US database, in this case, I'll treat it as the main database on the screen here, we can have the US database asynchronously update the India database, meaning every minute, every five minutes, every 10 minutes, the US database syncs up with the replica in India and vice versa, and they update each other.
>- Any updates that happen in the US database get done in the India database, and any updates that were done in the India database gets done in the US database.
>- And only then do the India users who are hitting the India database see my post.
>- And that means that we avoided having to do a roundtrip from the US to India when I initially posted the post on LinkedIn.
>- So I, as the US user, immediately saw my post appear on my feed, Maybe other US users immediately saw it appear on their feed.
>- Then our US database asynchronously updated the replica in India.
>- And a minute after I posted the post on LinkedIn, all of my connections or followers based in India saw my post in their feed.

>- Now here to be clear, this is not necessarily how LinkedIn is actually designed, but this is one way that you could design it, and this is one way that you could database replication to have better latency in your system in a place where you don't really care about asynchronous updates between your replicas.
>- You're fine with having your replicas not be up to date with each other at all times.
>- Of course there are many types of services and products for which you would not want that to happen, and that's why you may not always use this type of asynchronous replication.
>- But for certain use cases, it might be viable.

> Another example is imagine you work at a big tech company like let's say Google, and you're deploying a piece of software to production.
>- Maybe you've got multiple database replicas across the world that serve your piece of software to end users, but you probably don't need that new piece of software that you're about to deploy, like let's say a new binary or a new container image, maybe you don't need the results of this deployment to be experienced in all parts of the world where you've got your database replicas immediately.
>- So here you might also have asynchronous replication where you deploy the binary or the container image, and it gets written in one database, and then asynchronously will get written to all of the other databases.

> So that's replication.

#### Now let's look at another scenario (Sharding).
>- Imagine that you've got a system and in your system you have one main database.
>- And your system is serving hundreds of thousands, if not millions, of requests, and your main database is starting to get overloaded.
>- Your main database can't handle all of these requests at once.
>- It's becoming a bottleneck and throughput is just too low.

>- What could you do to improve this?
>- Of course you could try to scale vertically by making your database server beefier, but there's only so much that you can do with regards to vertical scaling.
>- So the natural next step is to scale horizontally, meaning to add database servers.
>- So maybe instead of having one database server, you're gonna have five database servers.
>- So similar to what is discsussed above, where we had a replica, maybe you're gonna have just five, or 10, or 20 replicas of the main database.
>- Now you've effectively increased the throughput by a factor of 10 or by a factor of 20.

>- But here we run into another issue.
>- What if our system is a system that's got tons of data?
>- Let's say that our system is something like Facebook, where we've got over a billion users, and imagine that we've got huge amounts of data.
>- Do we really wanna have all of that data replicated across a bunch of different databases? Maybe not.
>- Maybe that's not the most optimal way to do this.
>- So maybe what we could do instead is we can actually split up the data.
>- So just splitting up the data, rather than replicating it a bunch of times.
>- And this, this idea of splitting up or partitioning your data is what's known as sharding.
>- You split up your main database into a bunch of little databases, which are named shards or data partitions.
>- You've increased your throughput by doing this, and you've avoided duplicating so much data so many times by just splitting it up.

> Now of course the natural next question here is, how do you know how to split up the data? How do you know where to put certain chunks of data, in what shard to put certain chunks of data?

>- Well, here you've got a few options.
>- One option, if you're dealing with a relational database for instance that consists of tables is to actually split up your tables and to store certain rows in some shards, and other rows in other shards.

>- Now this can come with problems though.
>- Because as you can imagine, you might have what are known as hotspots, where certain shards get a lot more traffic than other shards just by nature of the data they store.

>- So of course here, a very reasonable way to split up your data is by using hashing.
>- You can use a hashing function, one that guarantees uniformity to determine what shard a piece of data is gonna get written to and read from.
>- Now of course here, since we're dealing with actual data stored in a database, you're not gonna wanna change your hashing function if you do this, because you need to make sure that reads and writes for a particular piece of data are always going to the same database server.

>- And here, by the way, consistent hashing might be kind of useful.
>- But if one of our existing database servers were to go down, consistent hashing wouldn't really help us.
>- If a database server goes down, then you have a problem, because your database is such a critical part of the system.
>- Consistent hashing is not gonna be the savior here.
>- In that case, you would probably wanna have actual replicas of each shard that could take over if a single shard goes down.

>- Overall, the point is that, depending on the type of data that you're sharding, you can decide how to split it up in different ways.
>- You just have to put some thought into it, and this is obviously something that you're gonna wanna do in a systems design interview.
>- The logic that dictates what shard a database read or write gets forwarded to, you could have it in your application servers.
>- The application server could have some logic, it might be literally be if-else statements to determine what shard it's gonna request that data from or it's gonna write that data to.

> But what you would probably prefer in practice would be not to have this logic at your actual server level, but instead maybe to have a reverse proxy that would act on behalf of your database servers.

> **All in all, replication and sharding are two very powerful tools that you're definitely going to use in your systems design interviews, especially when you're trying to make your system more performant.**

---

### 16. Leader Election
> Citizens in a society typically elect a leader by voting for their preferred candidate. But how do servers in a distributed system choose a master node? Via algorithms of course!

> This form of algorithmic democracy is known as "leader election", though we personally think "algorithmocracy" sounds way cooler.

#### 5 Key Terms

- ***Leader Election***
> The process by which nodes in a cluster (for instance, servers in a set of servers) elect a so-called "leader" amongst them, responsible for the primary operations of the service that these nodes support. When correctly implemented, leader election guarantees that all nodes in the cluster know which one is the leader at any given time and can elect a new leader if the leader dies for whatever reason.

- ***Consensus Algorithm***
> A type of complex algorithms used to have multiple entities agree on a single data value, like who the "leader" is amongst a group of machines. Two popular consensus algorithms are **Paxos** and **Raft**.

- ***Paxos and Raft***
> Two consensus algorithms that, when implemented correctly, allow for the synchronization of certain operations, even in a didstributed setting.

- ***Etcd***
>- Etcd is a strongly consistent and highly available key-value store often used to implement leader election in a system.
>- Learn more: [https://etcd.io/](https://etcd.io/)

- ***ZooKeeper***
>- ZooKeeper is a strongly consistent, highly available key-value store. It's often used to store important configuration or to perform leader election.
>- Learn more: [https://zookeeper.apache.org/](https://zookeeper.apache.org/)

---

>- Leader election is a relatively advanced topic of systems design in general computing.
>- Especially if you dive into the details of leader election.
>- But at a high level, it's actually quite simple to grasp.
>- Unfortunately for us, in the context of systems design interviews, all that you really need as far as leader election is concerned, is a high level understanding of it.
>- So having a high level understanding of leader election is gonna be a great tool for you to have in your tool belt when you walk into a systems design interview.

>- So imagine that you're designing a system for a product that allows users to subscribe to the product on a recurring basis.
>- For instance, you can think of Netflix, or of Amazon Prime, where users can subscribe on monthly or annual basis. They pay a monthly or annual fee for a product or service.
>- You could imagine that for such a system, you might have a database in which you're gonna store information about user subscriptions.
>- So for instance, you might store whether or not a user is currently subscribed to the service that you're offering.
>- You might store the date at which point the users subscription is suppose to renew.
>- You might store the price that the user should be charged on a recurring basis.
>- You might store all this information in your database. And then, you might be using a third party service that would be the service actually taking care of charging the users, of debiting funds from their bank accounts, of charging their credit cards or debit cards.
>- And here, you could imagine the maybe your third party service is PayPal or Stripe.
>- And of course, this means that your third party service needs to somehow communicate with your database. Because your third party service needs to know when a user should be charged again, how much they should be charged, etc.
>- Now, you may not want to have this third party service actually interact with your database directly.
>- First of all, that may not be possible because maybe the third party service can't actually be hooked up directly into your database. But even if that is possible, you may not want to do that.
>- Your database is a pretty sensitive part of your system. It contains important information, and you may not want to have some random third party service connect directly into it.

>- So, a reasonable thing to do, would be to inset some service in the middle, between the third party service and the database.
>- And this service would be in charge of basically talking to the database, maybe on a periodic basis. Figuring out when certain users subscription is gonna renew, how much that user needs to be charged. And then this service is gonna go to the third party service, to PayPal or to Stripe, and actually tell the third party service to charge the user.
>- So this service would be in charge of communicating with the database, of getting information back from the database, and then communicating with the third party service, and having the third party service actually charge users. And this seems reasonable.

>- But, as you might be thinking, this could pose a problem.
>- So presumably this service that lives in between the third party service and the database consists of one server. One machine. And if that's the case, if this service only has one machine or one server, then what happens if this one machine or one server fails? Cause remember, if we're dealing with a large-scale distributed system, we always have to expect that our machines, that our servers, are gonna fail.
>- And if this single server or single machine fails, then our entire payment system fails. That's obviously terrible.
>- Okay, so then the natural solution to that is to introduce redundancy in our system.
>- Specifically, redundancy in this service that lives in between the third party service and the database. So instead of just having one server, let's say we can have five servers.
>- And these five servers are gonna be the ones in charge of this whole business logic in between the database and the third party service.

>- But this introduces a new problem into our system.
>- The request going from the servers to the third party service, which probably tells the third party service to actually charge a user, to actually debit funds from their bank account.
>- This request is the kind of request that we definitely don't want to duplicate.
>- We only want to make that request, or perform that operation once.
>- And if we've got five servers in charge of this whole business logic here in the middle, how do we ensure that this request only gets issued, or that this operation only gets performed once?

> Well, this is where leader election comes into play.

>- With leader election, as the name might suggest, if you have a group of machines or a group of servers that are in charge of doing the same thing, instead of having all of them doing that same thing, which might not be something that you want to do multiple times, like in this case, you definitely don't want to make a request for a given user multiple times.
>- Leader election has the servers in question elect one of themselves as the leader. And that server, and that server alone, is gonna be the one responsible for doing the actions that all of the servers are kind of meant to do.
>- And if something happens to the leader, then one of the other servers is gonna become the new leader. A new leader is gonna be elected, and one of these other servers is gonna become that leader, and is gonna take over.

>- Well, it turns out that this seemingly simple task of having multiple machines, multiple distributed machines elect a single leader, and all be aware of who the leader is at any given time, and all be capable of re-electing a new leader if something happens to the original leader at any given point in time.
>- This is actually a very difficult problem to solve. The reason it's difficult, broadly speaking, is because when you've got multiple machines that are distributed, that need to essentially share state. In this case the state would be who the leader is. That's just difficult.
>- You never know what can happen in a network. What if there's a network partition? In other words, some network failure that makes some machines no longer be able to communicate with other machines. What happens then ? This concept of electing a leader is really non-trivial.
>- It's not so much the act of electing a leader. It's more the act of having multiple machines gain consensus, or agree upon something together. That's the real difficulty.
>- And here in this case, it turns out that that thing that these multiple machines are gaining consensus on is who the leader is at any given point in time. But it's the act of gaining that consensus, of sharing some state, in this case, who the leader is, it's the act of doing that that's difficult.
>- And so here, it turns out that, in order to actually achieve leader election, in order to actually do what we're describing, we can use what's called a consensus algorithm.

>- These consensus algorithms are these very complicated algorithms that are very mathematical, that allow multiple servers in a group, or more broadly speaking, multiple nodes in a cluster, to reach consensus, or to agree on some single data value.
>- And again, in the case of leader election, that single data value is gonna be who the leader is in a given group of machines or given group of servers. Or a cluster of nodes.
>- So, it turns out that there are a lot of these consensus algorithms out there. A couple of really popular ones are Paxos and Raft. These algorithms are very complicated and you're really never gonna be expected to implement them yourself in the industry.
>- Well it turns out that in the industry, typically you use some other third party service that itself might use Paxos or Raft under the hood to achieve leader election.

> There are these two tools called Zookeeper and Etcd.
>- Zookeeper and Etcd are these two tools that aren't necessarily primarily meant to be used for leader election, but that happen to allow you to implement your own leader election in a very easy way. And they're very often used in the industry.
>- For instance, at Uber, at least up until 2019, a lot of internal systems that Uber use Zookeeper to implement leader election.

#### What is Etcd ?
>- Etcd is a key-value store.
>- So literally a database that allows you to store key-value pairs.
>- But Etcd is highly available and strongly consistent.
>- And there aren't that many databases, let alone key-value stores, that are both highly available and strongly consistent.

> How does Etcd achieve high availability and strong consistency?
>- They do so using leader election, and more precisely, by implementing a concusses algorithm. A real concusses algorithm and it turns out that Etcd implements Raft. The Raft concusses algorithm.
>- Simply put, they're gonna need multiple machines that can read and write to the main key-value store that Etcd supports, because they need that high availability in case one machine dies, but they also need to make sure that they always have a single source of truth for the key-value pairs in the key-value store to achieve that strong consistency.
>- And so basically it's the same problem that we had here with our five servers, where we never wanted to have this request be duplicated, so the nodes under the hood in Etcd probably need to have one leader that's elected to take care of the rights in the key-value store, so they have to implement leader election, and they have to use a concusses algorithm to do so.
>- And this allows them to have a highly a highly available and strongly consistent key-value store.

>- We can then take advantage of that high availability and of that strong consistency to implement our own leader election in our system in a much simpler way.

---

### 17. Peer-To-Peer Networks
>- Equality for all.
>- Sharing is caring.
>- Unity makes strength.
>- The more the merrier.
>- Teamwork makes the dream work.
>- Welcome to peer-to-peer networks!

#### 2 Key Terms

- ***Peer-To-Peer Network***
> A collection of machines referred to as peers that divide a workload between themselves to presumably complete the workload faster than would otherwise be possible. Peer-to-peer networks are often used in file-distribution systems.

- ***Gossip Protocol***
> When a set of machines talk to each other in a uncoordinated manner in a cluster to spread information through a system without requiring a central source of data.

---

>- Peer-to-peer networks is a very cool topic in systems design and in general computing, it's a very interesting one. It's also relatively advanced which makes it all the more useful to know about for systems design interviews and that's why we cover it here on SystemsExpert.
>- So perhaps the best way to understand what a peer-to-peer network is and how it works, is to look at a use case.

>- And so here, I want you to imagine that you are designing a system for some big tech company where you're gonna want to be able to deploy or transfer large files to thousands of machines at once.

>- For example, a video file from security cam every 15 mins or so.
>- And since we're building this system for a big tech company, we can assume that the system is gonna live in a powerful data center owned by the big tech company and so we're gonna assume that our system has a total network throughput of 40 gigabits per second.
>- *And 40 gigabits per second comes down to five gigabytes per second. There are eight bits in one byte, so you divide 40 by eight and you get five gigabytes per second.*
>- This is a reasonable network throughput to assume for an advanced data center.
>- But okay, so now we've got all of our requirements and all of the info that we need to really understand how good the system really is and how well it's gonna operate, and so with just some simple math, we can see that at any point when we're wanna actually transfer a five gigabyte file, if we have a network throughput for our system of five gigabytes per second, and we wanna send the five gigabyte file to 1,000 machines, then this operation of transferring the file to 1,000 machines is gonna take 1,000 seconds.
>- It'll take one second to transfer the five gigabyte file to the first machine, another second to transfer the five gigabyte file to the second machine and so on and so forth, 1,000 times 1,000 seconds.
>- And 1,000 seconds comes down to roughly 17 minutes. 17 minutes is actually quite long for this type of operation, especially if you assume that we might do this repeatedly throughout the day.
>- Maybe we're gonna do this transfer of five gigabyte files every 15 minutes and that's really bad if we have this operation that takes 17 minutes.

>- So here we can clearly see that we have a **bottleneck** in our system.
>- So how could we improve this system?
>- Well, maybe instead of only having one machine serving these five gigabyte files, why don't we have multiple machines?
>- So instead of having only one machine serving these five gigabyte files, we're gonna have let's say, 10 machines serving these five gigabyte files.
>- And here we have our 1,000 machines that are now gonna be requesting the five gigabyte files in a distributed manner from these 10 machines.
>- And so assuming that our 1,000 machines do so in a very balanced way between the 10 machines here, and this would basically speed up our system 10 times over.

>- But we also run into a problem with this approach because, first of all, the speed of our operation of transferring a five gigabyte file still isn't great.
>- 17 minutes divided by 10 is still roughly a minute and a half, which isn't amazing.
>- It's not bad comparatively speaking, but it's not amazing depending on our use case it might actually be pretty bad.
>- But also that means that these five gigabyte files now need to be replicated on all of these 10 machines.
>- Do we wanna replicate that data across all of these machines ?

>- Maybe not, maybe there's a better solution.
>- What about **Sharding** ?
>- Maybe we could shard our five gigabyte files, in other words, we could have some of the files live in one machine, oher files live in another machine and so on and so forth.
>- But then we run back into the first issue of whenever we try to transfer one of the files, then all of the 1,000 machines are gonna be going to the same machine that has that particular file and we'll have once again a bottleneck and it won't be great, we'll be back with the 17 minute operation.

> ***So, so far all of our approaches are problematic and this is where peer-to-peer networks come into play.***
>- So let's see how we could improve this system using a peer-to-peer network.
>- When you're dealing with a peer-to-peer network, you call the machines in that peer-to-peer network, **peers**.
>- The idea is that they are peers that are gonna work together toward a common goal.
>- So we'll go back to the first solution, we just have one machine trying to send this five gigabyte file to 1,000 machines and we saw that we had a bottleneck.
>- Well, what if instead of sending this five gigabyte file to each and every one of the 1,000 machines, what if instead we were to split up this five gigabyte file?
>- We were to split it up into very small chunks, very small pieces of the five gigabyte file and then we were to send these chunks to all of our peers and then we were to let our peers communicate with one another to grab the missing chunks that they all need to create the final file and let them basically build up their own total file.
>- *That is the general gist of a peer-to-peer network.*

>- More concretely, in this example, let's imagine that we were to divide our five gigabyte file into 1,000 five megabyte files.
>- So divide 5GB into 1,000 and you get a bunch of 5MB files.
>- Imagine that we were to send out one five megabyte file per machine.
>- Since we have 1,000 five megabyte files and 1,000 machines, we could send out one five megabyte file to each machine.
>- This would take one second because 1,000 five megabyte files is five gigabytes.
>- It's effectively our five gigabyte file and if we have a network throughput of five gigabytes per second, then we can send five gigabytes in one second, we can send 1000 chunks of five megabytes in one second to 1,000 machines.

> And here we're ignoring the overhead of establishing connections over the network or of handling network partitions. We're gonna put that aside for now 'cause that doesn't really matter that much to understand peer-to-peer networks.
>- So we can transfer these 1,000 five megabyte files in one second and then you can imagine that for a single machine to get the entire five gigabyte file, if a single machine has one five megabyte file, it now needs the 999 other five megabyte files.
>- And so, a single machine needs to talk to the 999 other machines to get all of the missing pieces that it doesn't have.

> How long would this take for a single machine to do?
>- It would take 0.999 seconds, one second divided by 1000 multiplied by 999.
>- So for a single machine, it would take one second to get the rest of the five gigabyte file from all of the other machines.
>- But the beauty in this is that, when two machines out of 1000 machines talk to each other, two other machines can talk to each other at the same time.
>- The idea is that here you can parallelize five megabyte transfers because while two of your machines are talking to each other and one of them is transferring five megabytes of the file, two other machines can simultaneously talk to each other and have one of them transfer five megabytes of the file.

>- So the idea is, compared to our first solution where we had the single machine, sending five gigabytes to one machine, then to another machine, then to a third machine, and we had this bottleneck.
>- Whereas with our new tentative solution, the peer-to-peer network solution, we have a bunch of arrows or a bunch of communications happening all at once.
>- That's how a peer-to-peer network works at a high level.
>- So this is how the **gossip protocol** or **epidemic protocol** basically works.
>- And this idea of having pieces of information that are effectively mappings, effectively pieces of a hash table, this is actually known as a **D**istributed **H**ash **T**able (**DHT**).

>- Peer-to-peer networks often operate by having a distributed hash table of what peers hold what pieces of data.
>- But so all in all, this is how peer-to-peer systems work.
>- They're very fast and they have lots of applications.
>- One good example is a system called Kraken that was created by Uber and that's used at Uber.

>- And really one way to think about it, conceptually to think about why this is so, so much better than our naive solution that we talked about at the beginning is just because of all of the connections that you can establish between peers when you have the peers communicating with one another instead of when you have them just communicating with one single machine.

> And on a final note, peer-to-peer networks really have far reaching applications.

> Beyond the above examples, one example of the peer-to-peer network application that you may very well be familiar with is the example of ***torrenting***.
>- Torrenting basically involves one person or one machine that has a piece of data, typically a large file like a movie and spreading that file in chunks to a bunch of peers, to a bunch of other machines all over the world, presumably.
>- And then having these peers work together to obtain all of the missing pieces that they need to puzzle them back together and then to finally get the end product, the full file.

>- And amongst other things, what it accomplishes is that, that main person or main machine that had the original file, doesn't need to send the full file to thousands or hundreds of thousands of people, all that it needs to do is send all of the chunks of the file and then the peers are just gonna take over.

---

### 18. Polling And Streaming
> You can think of polling and streaming kind of like a classroom; sometimes students ask the teacher lots of questions, and other times they quiet down and listen attentively to the teacher's lecture.

#### 2 Key Terms

- ***Polling***
> The act of fetching a resource or piece of data regularly at an interval to make sure your data is not too stale.

- ***Streaming***
> In networking, it usually refers to the act of continuously getting a feed of information from a server by keeping an open connection between the two machines or processes.

---

>- So far, we've dealt with systems where and servers communicated with each other by having clients issue requests to servers and having servers send responses back to the clients.
>- What happens when we're designing a system where our clients are gonna want a piece of data that gets updated or that changes very regularly?
>- As an example, imagine that you were building a system where your clients are gonna have to be able to monitor the temperature outside for example.
>- The temperature outside is gonna change a lot, your servers are gonna have this changing data and your clients are gonna need to see all these changes.

>- Or similarly, let's assume that you're building a system that consists of a chat app where you have individuals or clients that are meant to be able to communicate with each other in real time, send the messages to each other in real time.

> In both of these examples, we're dealing with data, temperature data or messages that gets updated regularly and that clients are gonna need to see updated regularly.

> How would we build a system to reflect these regular updates, to get these regularly updated pieces of data?
> Well, this is where polling and streaming come into play.

> Polling and streaming are two techniques that are gonna allow you to do just that.
> They're gonna accomplish very similar things with a few nuances and they're gonna be great techniques to have in your tool belt when you walk into a systems design interview.

> ***Polling*** is actually very very simple both to grasp and to implement. The idea behind polling is that the client is gonna issue a request for data that it wants on a recurring basis, following a set interval.
>- The interval can be every second, 2 seconds, every minute etc., depending on the use case.
>- Polling is very simple.
>- All that you are doing is having your client issue a request on a recurring basis following some interval and that's it.
>- Polling is really good because it definitely allows us to support some of our use cases like for instance, the temperature use case that we mentioned before.
>- If we wanted our clients to monitor the outside temperature and that temperature was stored in our servers, but it changed frequently than we would probably want to have our clients poll for the temperature, let's say every 30 seconds, or every minute or every hour.
>- That would seem like a reasonable thing to do.

>- But as you can probably already tell, polling has limitations because what if we go with the example of a chat room?
>- When you're chatting with someone online, let's say on Facebook messenger or on WhatsApp, you're gonna want to receive messages from other people instantly.
>- And here polling might have some limitations because let's say you were polling for new messages in your chat app every 30 seconds for instance, that would obviously not lead to an instantaneous experience.
>- You would basically have users or clients see some messages and then see nothing for 30 seconds or rather no update, no new messages for 30 seconds and if the person they were chatting with sent them a message or multiple messages in those 30 seconds, they would only see them after the 30 seconds. So that would be a really bad experience.
>- Now of course you can try to fix that with polling by basically reducing the amount of time that elapses between requests.
>- So for instance, you could issue requests to get messages from your servers every one second or every 0.5 seconds, every 0.1 seconds.
>- The more you reduce, the time between the requests when you're implementing polling, the more instantaneous of an experience you will get. So suddenly our chat app, actually does become satisfied. We do have an acceptable chat app.

> But that comes with the **trade-off** of having a lot of load on your server.
>- Because you can imagine if you're polling, let's say every 0.1 second because if you really wanna give that instantaneous feeling for a chat app, you're gonna wanna poll even multiple times per second. So let's go with every 0.1 seconds.
>- That means that you're gonna be issuing 10 requests per second for one client.

>- Now imagine the system at scale, suddenly you've got, thousands, tens of thousands, potentially even millions of users issuing 10 requests per second just to get messages.
>- That's a lot of load, to put on your server, and so that's where polling starts to lose some of its appeal and that's where streaming comes into play.

> The way that ***streaming*** works is instead of having your client repeatedly request data from your server, you're gonna have your client open a long lived connection with your server and typically this is done through what's called a socket.
>- A socket is basically a file that lives on your computer that your computer can write to and read from, to communicate with another computer, in a long lived connection kind of way.
>- You can loosely think of a socket as a portal into another computer, into another machine that you can reach through or rather communicate through if you wanna have two machines communicate with each other without having to repeatedly send requests.
>- Just an open connection that lives so long as neither of the two machines close it or so long as the network is healthy.
>- Going back to the example of chat app, your server would push messages, new messages, through this connection, to your client and that's gonna be, the streaming in action.
>- So basically your client is streaming data, from your server.
>- Now the key point, to retain about streaming is that unlike with polling where your client is the one requesting data from your server and your server only sends data to your client, when it receives a request, with streaming, your client is merely saying, *"Hey server, I'm listening to you if you wanna give me data, I'm not requesting for data, I'm just listening, I'm here, you can talk to me."*
>- And then it is the server's job to actually send that data out to the client, whenever the server wants to or whenever the server has an update here basically you have to implement your business logic, on the server side.
>- Your server will no longer be the sort of passive thing in your system instead, it'll have to proactively send data to the client.
>- And by the way, you may have heard the term pushing used before and if not, you are hearing it now, people will often call this act of having servers send data proactively so, to clients as pushing. Instead of basically waiting to get a request, they will proactively push data, to clients.

>- What streaming allows you to do, is it allows you to have a continuous stream of data.
>- So if we're going back to the example of the chat app, it would allow your clients to continuously receive new messages so long as our server correctly pushes new messages the second that it gets them but it would allow your clients to continuously get these new messages without having to repeatedly request them from your server.
>- And so suddenly you can have that instantaneous experience in your chat app without having to issue 10 requests per second, per client, but just by having, one long lived connection, per client.

> *Now it is important to note that streaming is not necessarily better than polling, here based on the chat app example, streaming definitely comes across as superior to polling. But the truth is, depending on your use case, depending on the product or service that your system supports, polling might actually be better than streaming or of course streaming might be better than polling. So here's its gonna be your job in a systems design interview to understand what functionality your system is gonna support and to then decide accordingly whether you should use polling, streaming or neither.*

> The general rule of thumb is gonna be that if you need some instantaneous experience or if you need data updated, very frequently, then you're likely gonna use streaming but if you need data updated not too frequently, maybe every 30 seconds, maybe every minute, maybe every five minutes, then polling might be more useful.

>- So if you're building a system for currency exchange, maybe you're gonna need live updates to your currency pairs, to the prices of currencies, then you're probably gonna wanna use streaming.
>- If you're building a chat app and you need that instantaneous type of experience then you're probably gonna need streaming, but if you're building maybe a dashboard that monitors stock prices but more to give you a snapshot of stock prices at any given point in time, but not necessarily to allow your users to do live trading, then maybe you don't need to stream there because maybe you only need your prices updated every 30 seconds or every five minutes and so there you might prefer polling or maybe you're building that application that monitors temperature changes, in that case you might prefer polling because there might be no real need to have an open connection, at all times between clients and servers in that case.

> The main thing is that you're gonna wanna know what functionality, your system has to support, and depending on that, you're gonna have to decide whether you wanna go with the polling approach, a streaming approach, or something entirely different.

---

### 19. Configuration
> The config file is like the genome of a computer application; it stores parameters that define your system's critical settings, much like your DNA stores the genes that define your physical characteristics.

> Unlike its biological counterpart though, the config file is easily editable. No gene therapy needed!

#### 3 Prerequisites

- ***JSON***
> A file format heavily used in APIs and configuration. Stands for **J**ava**S**cript **O**bject **N**otation, Example:
```
{
	"version": 1.0,
	"name": "AlgoExpert Configuration"
}
```

- ***YAML***
> A file format mostly used in configuration. Example:
```
	version: 1.0,
	name: AlgoExpert Configuration
```

- ***Key-Value Store***
> A Key-Value Store is a flexible NoSQL database that's often used for caching and dynamic configuration. Popular options include DynamoDB, Etcd, Redis and ZooKeeper.

---

#### 1 Key Term

- ***Configuration***
> A set of parameters or constants that are critical to a system. Configuration is typically written in **JSON** or **YAML** and can be either **static**, meaning that it's hard-coded in and shipped with your system's application code (like frontend code, for instance), or **dynamic**, meaning that it lives outside of your system's application code.

---

>- Configuration is a very simple part of systems design.
>- And it's often overlooked because of it's simplicity, but despite it's simplicity, it is very important.
>- In fact, most large scale distributed systems are gonna be relying a lot on configuration, so it's very important for you to know how configuration works, to know what it is, and to have it as a tool in your tool belt when you are in a systems design interview.

- **So what is configuration?**
>- Well, to put it simply, configuration is a set of parameters or a set of constants that your system or application are going to use.
>- But instead of having these parameters or these constants deeply intertwined in your code, you're going to write them or configure them elsewhere in a seemingly isolated file.

>- Typically, configuration is written in JSON format or in YAML format.
>- This makes it very easy to read and to edit regardless of the language that your underlying application is using or written in.
>- So really, a very simple way to think about configuration is just a set of constants that you use in your application.
>- And this is why configuration is often overlooked because it seems so simple at face value.

>- Now, one thing that's important to note about configuration is that they're two primary types of configuration.
>- There's what's known as ***static configuration***, and what's known as ***dynamic configuration***.

>- Static configuration is configuration that's gonna be bundled or packaged with your application code.
>- So, basically what that means is that, if you wanna change some configuration, you should deploy the entire code because the config file would be packaged with your code.
>- This is both pros and cons.

>- Some of the pros are that, typically, when you submit a change to your code base, it's gonna go through a thorough code review process.
>- At least if you're working as part of a large team that has proper code review practices set up.

>- This means that if your configuration change happens to break your application, that breakage will likely be caught in tests that you might have written or in quality assurance testing that might happen before you deploy your application.
>- So basically, static configuration tends to be a little safer, but it's also gonna make it a little bit slower to see changes related to your configuration happen because you'll have to wait for your entire application to be redeployed.

>- On the other hand, dynamic configuration is configuration that is completely separated from your application code.
>- This means that you can change your configuration and at a moment's notice, the configuration changes are gonna take effect and have ramifications on your system.
>- So, dynamic configuration is a little bit more complex because it naturally has to be backed by some sort of database that your application or your system is gonna be querying to see, basically, what the current configuration is.

>- But then, dynamic configuration gives you a lot of power and flexibility because you can imagine you could actually build a user interface, a UI, on top of your configuration which can then allow your team, your engineers, your systems administrators to make changes to the configuration with the click of a button.

>- Now as you can imagine, this comes with both pros and cons.
>- The pros are that you can make changes to your configuration and see those changes take effect or have an impact very quickly, meaning that you can deploy new features or deploy new things very fast.
>- But, this also comes with a lot more risk.
>- Suddenly, you might not have a lot of thorough review when someone wants to make a configuration change.
>- You might not have tests that run when your configuration changes, and that might be bad for your system as a whole.

>- Now, what ends up happening typically in big companies is that you do have dynamic configuration because it comes with so many benefits, but then you build tools around that dynamic configuration to still make it safe.
>- So for instance, you might build a review system on top of the configuration user interface.
>- You might implement access controls to only allow certain people in your organization to make configuration changes.
>- You might even build deployment systems around configuration.

>- At large companies like Google, you can build very complex systems such that when you make a configuration change, it only gets deployed to maybe 1% of users or 10% of users.
>- That way, even though your configuration change has impact on your application very quickly, it only effects a few users.
>- That way, you can more safely roll out changes externally.

>- So basically, the key point to take away from dynamic configuration is that it gives you a lot of power, but to quote our friendly neighborhood Spiderman, with great power comes great responsibility.
>- And having a system that relies on dynamic configuration often means that either you really have to have that great responsibility or you have to build slightly complex tools to enforce that great responsibility on your team and organization.

---

### 20. Rate Limiting
>- *Poke*
>- *Poke*
>- *Poke*
>- *Po--*

> Too many pokes! You just got rate limited.

#### 4 Key Terms

- ***Rate Limiting***
> The act of limiting the number of requests sent to or from a system. Rate limiting is most often used to limit the number of incoming requests in order to prevent **DoS attacks** and can be enforced at the IP-address level, at the user-account level, or at the region level, for example. Rate limiting can also be implemented in tiers; for instance, a type of network request could be limited to 1 per second, 5 per 10 seconds, and 10 per minute.

- ***DoS Attack***
> Short for *"denial-of-service attack"*, a DoS attack is an attack in which a malicious user tries to bring down or damage a system in order to render it unavailable to users. Much of the time, it consists of flooding it with traffic. Some DoS attacks are easily preventable with rate limiting, while others can be far trickier to defend against.

- ***DDoS Attack***
> Short for *"distributed denial-of-service attack"*, a DDoS attack is a DoS attack in which the traffic flooding the target system comes from many different sources (like thousands of machines), making it much harder to defend against.

- ***Redis***
> An in-memory key-value store. Does offer some persistent storage options but is typically used as a really fast, best-effort caching solution. Redis is also often used to implement **rate limiting**.

> Learn more: [https://redis.io/](https://redis.io/)

---

>- Rate limiting is a pretty simple concept to grasp, but it's very important in systems design especially when dealing with large-scale systems.
>- Mainly because it has a lot of ramifications including security ramifications and performance ramifications.
>- So to put it simply, rate limiting is basically setting some sort of threshold on certain operations, past which these operations will return errors.
>- Or an even simpler way to put it is, rate limiting is limiting the amount of operations that can be performed in a given amount of time.

>- So if we look at a very simple system, we've got a client or a set of clients that interact with a server or a set of servers and then the servers speak to a database.
>- Which returns data to the servers which then returns the data back to the clients, very simple system.
>- And so if you wanted to rate limit this system, you could imagine that maybe you would say, I only want to allow let's say two requests every 10 seconds in this system.
>- So if a client issued a request to the server, the server would say, *"Okay this is the first request in 10 seconds, I'm gonna go to the database."*
>- The database would return data and then the server would return that data back to the client.
>- Then a second request would come through, the server would say, *"Okay, second request in 10 seconds, that's fine I'm gonna go to the database."*
>- The database would return the data and then the server would return that data to the client.
>- And then if the client or one of the clients issued a third request within those 10 seconds, the server would say, *"Wait a second, we don't allow more than two requests within 10 seconds, so I'm immediately gonna return an error."* I'm immediately gonna say, *"Hey, you've issued too many requests, I can't handle this right now."*
>- And if the clients continued to issue requests within these 10 seconds, the server would continue to return errors, saying, *"Hey we won't accept these requests right now."*

>- Now the reason rate limiting is so important is that if you don't rate limit certain operations in a system, you run the risk of having your system basically be brought down by malicious actors.
>- There's a very common attack in systems design or in computing in general rather known as a Denial of Service attack or a DOS attack D-o-S.
>- And what a Denial of Service attack is, is when a bad actor floods a system with a bunch of requests, a bunch of traffic and basically brings the system down.
>- Because the system can't handle traffic anymore or can't handle it properly, can't handle it as fast as it should be, because basically the bad actor is clogging the system.
>- The system doesn't have enough throughput to handle all of the traffic.

>- Rate limiting can help prevent that from happening, because rate limiting will protect you from getting flooded with traffic.
>- Past a certain point you'll just throw back errors and say, *"Nope we're not handling this, we're not gonna go clog or database or clog our servers with this stuff, we're just gonna return errors."*

>- And so a **good example** of rate limiting in real life or in a real system is on AlgoExpert for our code execution engine.
>- As you might imagine, we don't want users to be spamming the code execution engine needlessly.
>- So we have some rate limiting in place to prevent users from doing just that.
>- Because we don't want people to abuse the system and to spam the run code operation.

>- But to be clear, rate limiting is useful for all sorts of operations, not necessarily obviously taxing operations like running code on AlgoExpert.
>- Even things like issuing a request to get a web page can be operations that would be worth rate limiting.
>- And by the way, you can rate limit on a bunch of different things.

>- For instance, you can rate limit based on users. For instance you will identify a certain user that a request is coming from, and you'll do so maybe by looking at headers in a request, you might see authentication credentials that'll allow you to identify the user or something else.
>- But once you've identified the user you'll say, *"Okay, for this particular user, we will rate limit an operation at let's say, three operations per minute."*

>- You could also rate limit on IP address, you could rate limit on region, you could rate limit on your entire system as a whole.
>- For instance you might say, *"Hey we don't want our servers to ever handle more than 10,000 requests per minute. So if we ever exceed that number, we're just gonna start returning errors."*
>- Maybe this is because you have some sort of internal quota that you have to satisfy, and you just cannot handle more than 10,000 requests per minute.
>- Maybe it's for another reason, maybe you wanna prevent a certain region of the world or a certain organization that falls under the same IP address from abusing your system.
>- Who knows but the point is you can rate limit on a bunch of different factors or things.

> ***It is important to note that rate limiting, while very important and very effective, isn't the ultimate way to protect your system from attacks.***
>- If we're talking about Denial of Service attacks, while simple Denial of Service attacks may be thwarted by rate limiting.
>- If your system becomes the target of a more complicated attack like, a Distributed Denial of Service attack, a DDoS attack, then things get a lot more complicated.
>- Because a DDoS attack tries to circumnavigate something like rate limiting, by having a bunch of different machines that might not be identifiable as being part of the same organization or the same group and having all of these machines, inundate your system with traffic.
>- And then it becomes a lot tougher to be able to rate limit because you can't necessarily recognize that those machines are working together.
>- So that's just something important to keep in mind and this is why you still see to this day, huge companies, huge systems like Wikipedia or Blizzard Entertainment, the video game company that get their servers brought down by DDoS attacks.

>- In distributed systems, you typically handle your rate limiting not in-memory in your servers but rather in a separated service or database that all of your servers are gonna be able to speak to you.
>- And so one popular option for this that is actually used on AlgoExpert, is something called Redis.
>- You can think of Redis as an in-memory key value database or key value store, that can be used for rate limiting.
>- And basically when your clients would issue requests to your servers, your servers would first check Redis.
>- It would first check Redis and say, *"Hey, are we doing fine from the rate limiting point of view?"*
>- Then Redis would respond and say, *"Hey we're doing fine or Hey, we're not doing fine."*
>- And if you're not doing fine which means that you've hit the maximum amount of operations in a given time, then your server would go back to the client with an error.
>- Or if you haven't, if you're fine you're doing fine, you're under the threshold, then your server would go to the database, and then of course the rest of the operation would go smoothly from there.

>- Okay and the last thing that's important to know about rate limiting is that you can make your rate limiting a lot more complicated than what we've seen here.
>- So far we've just looked at rate limiting operations based on a single number of operations, in a given amount of time.
>- Like in our example before, one request every five seconds. But you could imagine that depending on your use case, you might want a rate limit a little bit differently.

>- So let's look at the use case for us on AlgoExpert with the code execution engine.
>- On the one hand, we don't want users to spam the run code button or to spam the run code operation. Because that just doesn't make sense and it would not be good for our system.
>- On the other hand, we do want users to be able to press the run code button repeatedly. Because you can imagine that that's a nice thing for users to be able to do, at least to press the run code button maybe twice or three times in a row consecutively very quickly.
>- That's something that you might want to allow your users to do.
>- So maybe we're gonna say, *"Okay we'll rate limit the run code operation to once every 0.5 seconds."*
>- That way a user will not be able to really abuse it and spam the run code operation non-stop. But they'll be able to do it, every 0.5 seconds, so they'll be able to click it a few times in a row.

>- But then you might tell yourself, well wait a second that's good, we don't allow them to completely abuse it and spam it, but they'll still be able to spam it every 0.5 seconds.
>- So you could imagine that a user could just stay there and click the run code button, or write a script that hits our API every 0.5 seconds and that wouldn't be great.

>- So maybe we're gonna also put another limit, to I don't know, let's say three operations, three run code operations in the span of 10 seconds.
>- So we have tiers, we say you can only run code every 0.5 seconds, but you can only run code three times in 10 seconds.
>- And then you might have an even bigger tier, of say, you can only run code 10 times in one minute, because beyond ten times in a minute, there's something fishy going on.
>- You're clearly no longer just using the platform as intended, you're trying to do something malicious or something weird.

> So this concept of tier-based rate limiting, is a thing and it's very important. You can definitely imagine use cases where you would want to do that.
>- The only thing to keep in mind is that it complicates your rate limiting a lot.
>- Your rate limiting is gonna be a lot more complicated to code out than the simple example that we had earlier.
>- You'll have to keep track of windows of time and perform a lot more logic in your code.
>- It's certainly doable but it's a little bit more complicated.

---

### 21. Logging And Monitoring
> In order to properly understand and diagnose issues that crop up within a system, it's critical to have mechanisms in place that create audit trails of various events that occur within said system.

#### 3 Key Terms

- ***Logging***
> The act of collecting and storing logs--useful information about events in your system. Typically your programs will output log messages to its STDOUT or STDERR pipes, which will automatically get aggregated into a **centralized logging solution**.

- ***Monitoring***
> The process of having visibility into a system's key metrics, monitoring is typically implemented by collecting important events in a system and aggregating them in human-readable charts.

- ***Alerting***
> The process through which system administrators get notified when critical system issues occur. Alerting can be set up by defining specific thresholds on monitoring charts, past which alerts are sent to a communication channel like Slack.

---

>- Logging and monitoring are another two concepts or things in systems design that are very simple, very easy to grasp but that are nonetheless very important.
>- Especially as your system grows larger and larger with more and more users.

#### What is logging?
>- Well, first of all lets look at a scenario that you might find yourself in if you are building a system or rather managing a system.
>- Let's imagine that you are running a website like AlgoExpert, meaning a service where you sell some sort of product and you charge users money for that product.
>- You could imagine that as your system grows larger and larger, one day you might have a customer reach out to you and tell you, *"Hey, I just tried purchasing your product, I got a success message, telling me that I did in fact purchase your product. My credit card got charged, but I don't have access to the product. I tried refreshing the page, I don't have access. What is going on?"*
>- And of course, this would be a really bad issue and its the type of issue that might be tough to understand because you might be thinking, well this has never happened before, we've got tens of thousands of users, no one has ever experienced this, we're not sure how to reproduce this.
>- We can't really tell the customer, *"hey could you retry purchasing the product."*
>- We have no real visibility into what caused the issue, but clearly this seems like a very edge case issue, something that happens only once every so often but it's still a very bad issue.

>- How would we go about debugging this? And of course, this is where logging comes into play.
>- If you were dealing with this type of issue in lets say a coding interview problem, or as you were developing your service, as you are writing your front end code or as you are writing your API, you would likely debug this issue by putting logs.
>- If you are writing in Python, you would put print statements. If you are writing in JavaScript, you would use the console.log function.
>- The point is, you would log stuff to get more information about your code and to try and debug this issue.
>- And so here with your customer who got incorrectly charged, wouldn't it be great if you had access to logs related to that user's operations, or that user's behavior.
>- Logs that showed you what exactly happened when they tried purchasing your product and got charged, even though they weren't given access to your product.

>- And so in the context of systems design, we talk about logging, we are referring to literally logging stuff in your code, but we're also referring to somehow, having some sort of system or service in place that is going to collect all of your logs and store them in some kind of database so that you can go to that database and look through the logs at a later time to debug issues like this one that we just talked about.
> That's what logging is.

>- And so the way this works in practice is when you're writing your application code, you're going to put log statements in your code to log important information, things like errors, or important operations or requests that your users are performing and depending on the language that you are writing your application in, you might use a special library to format these logs because you really want to make sure that your logs have as much useful information in them as possible and so here two popular formats for logs that are often used in systems are Syslog or JSON.
>- So you would sprinkle your code with these logs and then you would have a service that collects these logs and stores them in some database.
>- So all that to say, logging while very simple, is incredibly important because it's what will allow you to actually debug issues at scale when you're dealing with a huge system.
>- And typically, if you work at a large company, or at a company that has rigorous engineering practices in place, you are going to have to have logs in your system.

#### What is monitoring?
>- Monitoring is similar to logging in the sense that it's a tool or a thing that makes managing a system a lot easier and a lot better.
>- You could imagine that if you've built a system that's growing, that's becoming bigger and bigger with more and more users.
>- You are going to want to have visibility into your system's health, your system's performance, your system's general status.
>- And how can you have that visibility? By making sure that you've designed your system in such a way that you gather meaningful metrics and that you have tools to monitor those metrics.

>- So for instance, imagine that you've designed and built a system like AlgoExpert. You could imagine that as AlgoExpert grows and grows, you're going to want to have visibility into a lot of operations on AlgoExpert.

> For instance, you might want to be able to see how your code execution engine is doing. Are users getting a lot of errors when they're running code? Are users getting a lot of latency when they're running code? What about your payment service? What about your authentication service? How many sales are you getting per week, per day, per hour? How many people are logging into your platform every day? What authentication service are they using? Is Facebook authentication more popular? Is GitHub authentication more popular? Google authentication, all of these things are the kinds of insights that you could imagine might be useful if you are designing, building and maintaining a system like AlgoExpert.
>- So basically, in the context or systems design and systems design interviews, monitoring comes down to making sure that in your overall system you've got systems in play to monitor important metrics about your overall system.
>- And so there are a lot of ways that you can gather metrics, one of them, which is kind of simple is to build some sort of service or perhaps you can use a pre-built tool that'll do that for you.
>- To scrape your logs, so you have to make sure that you've got robust logging in place. And to create metrics out of them.
>- As you can imagine, your logs might contain information that you could use to create meaningful metrics about your system.
>- Now the problem with this is that, first of all you are limited by your logs. In other words, you need to make sure that your logs contain the information that you want visibility over in your metrics.

>- As an example, if you want to measure the latency of specific requests in your system, you need to make sure that you log the latency of each request in your system.
>- An another limitation of this way of gathering metrics is that, if you ever decide to change your logs, you risk breaking your metrics system or your monitoring system and that's obviously not ideal.
>- So another popular way of gathering metrics is to use a time-series database, which is basically a specialized database specifically tailored for data that is related to time or data that might be measured over time and a few popular examples of time-series databases include InfluxDB, Graphite, Prometheus.

>- But so the point is, you use these specialized databases and you have your servers periodically send metrics to these databases or to this one central database that you might have.
>- And then you can query that database and usually that involves using a special query language.
>- You can also use tools that'll make pretty graphs out of the values stored in the database.

> And what's great about gathering metrics is that you can really build robust monitoring services that you can customize and they're not necessarily tied to your logging service or your logging system, so this can be a nice serve at perhaps more involved way of building monitoring into your system.

> And then one final thing that also important to note is **alerting**.
>- When you do have nice monitoring built into your system, you could imagine that you want this monitoring to be really useful for you.
>- So for instance, if you are looking at error rates, you might want to know when your error rates spike up past the threshold that you would deem unacceptable.
>- And so ideally, you would want to be alerted when something like that happens.
>- And this is where you can pretty cool things like for instance, you can hook up your monitoring system into something like Slack, the popular chat app that a lot of companies use.
>- So you can hook up your monitoring system in there such that when there is something that you deem valuable or important to know about, it will alert you.
>- It'll send a message on Slack, telling you, *"hey you've gotten two purchase errors in the past minute, something might be wrong, go check it out. Or hey, the average latency of your last a hundred run code operations on AlgoExpert exceeded two seconds. This is something that's abnormal, go check it out."*

>- So having a great alerting system can go hand in hand with having a great monitoring system.
>- All in all, logging and monitoring are two pretty simple concepts to grasp they can become really important when you've built a big system.
>- They're the kind of things that might not be important on day one when your system doesn't have that much activity or that much usage but they're also the kind of things that can quickly become extremely important as you grow, because if you do ever find yourself in the situation for instance where the customer got incorrectly charged or if you find yourself in a situation where you've got a bunch of errors but you don't know about them because you don't have proper monitoring in place.
>- Then your not going to be in a good situation.

> So in a systems design interview, while logging and monitoring might not be the most critical components of the system that you're designing.
> They're great tools to have in your tool belt to really polish your system and to make it the best system possible.

---

### 22. Publish/Subscribe Pattern
> Publish/Subscribe. Press/Tug. Produce/Consume. Push/Pull. Send/Receive. Throw/Catch. Thrust/Retrieve.
> Three of these can be used interchangeably in the context of systems design. The others cannot.

#### 4 Key Terms

- ***Publish/Subscribe Pattern***
> Often shortened as **Pub/Sub**, the Publish/Subscribe pattern is a popular messaging model that consists of **publishers** and **subscribers**. Publishers publish messages to special **topics** (sometimes called **channels**) without caring about or even knowing who will read those messages, and subscribers subscribe to topics and read messages coming through those topics.

> Pub/Sub systems often come with very powerful guarantees like **at-least-once delivery, persistant storage, ordering** of messages, and **replayability** of messages.

- ***Idempotent Operation***
> An operation that has the same ultimate outcome regardless of how many times it's performed. If an operation can be performed multiple times without changing its overall effect, it's idempotent. Operations performed through a **Pub/Sub** messaging system typically have to be idempotent, since Pub/Sub systems tend to allow the same messages to be consumed multiple times.

> For example, increasing an integer value in a database is *not* an idempotent operation, since repeating this operation will not have the same effect as if it had been performed only once. Conversely, setting a value to "COMPLETE" *is* an idempotent operation, since repeating this operation will always yield the same result: the value will be "COMPLETE".

- ***Apache Kafka***
> A distributed messaging system created by LinkedIn. Very useful when using the **streaming** paradigm as oppossed to **polling**.
> Learn more: [https://kafka.apache.org/](https://kafka.apache.org/)

- ***Cloud Pub/Sub***
> A highly-scalable Pub/Sub messaging service created by Google. Guarantees **at-least-once delivery** of messages and supports "rewinding" in order to reprocess messages.
> Learn more: [https://cloud.google.com/pubsub/](https://cloud.google.com/pubsub/)

---

> In order to fully understand the pub/sub pattern, and in order to appreciate its use, we have to remind ourselves of another concept in systems design, which is streaming.
>- Where we would have clients establishing long-lived connections with servers and effectively listening for data from those servers. In the case of our chat application, that data consisted of messages, like texts sent from a user.
>- Now that example worked very well for that super simple system, but what would happen if we wanted to expand that system? What would happen if we wanted that system to become a large-scale distributed system, which is likely what we would want, if we were building a real product.
>- Well, we would probably encounter some issues pretty quickly. Because the second that our system becomes a distributed system, we have to start asking ourselves, how are we gonna handle network partitions, for example? What do we do if our clients lose their connection with the servers? What do we do if our servers die? What happens to the messages? Do the messages just disappear? Will our clients be able to retrieve messages if they've lost a connection?
>- These are all really important questions. And in a lot of large-scale systems, the answer to that is, those messages stay, we have access to those messages, somehow, our clients are indeed able to retrieve those messages.

>- And perhaps here the chat application (discussed in the above topics) is not the best example because it doesn't really invoke a sense of hyper importance or urgency, but let's say we were dealing with a stockbroker.
>- And we had clients who were streaming or listening to servers for data about stock prices, and they were relying on those stock prices to execute really important trades with a lot of money on the table.
>- What would happen if there were network partition? Well, we certainly wouldn't want to suddenly lose access to a bunch of data/stock prices.

>- So what I'm hinting at here is that the second that we get into distributed systems, we start to have to deal with persistent storage for a lot of parts of our system. Because if we want our clients to be able to retrieve some form of data, then that data will almost certainly have to have been stored in persistent storage.
>- So at this point, you might be thinking, okay, great, just store the data in a database.
>- But a database might not be what you necessarily want, or at least your typical database might not be what you necessarily want, for any and all applications.
>- Maybe the data that we're really concerned with storing here is some form of asynchronous operation, like imagine a client basically triggers an asynchronous operation, some operation that doesn't block them from doing other stuff, and that operation, goes to the servers and then has to take some time to happen and then eventually, once it completes, it has to go back to the client or the response of that operation, the result of that operation, eventually, once it completes, has to go back to the clients.

>- That might not be something that you would wanna store in your typical database solution. So maybe at that point, you're thinking, well, okay, why don't we implement some form of storage solution at our server level, the servers that our clients are streaming from, or the servers that our clients are issuing these asynchronous operations to, but then you start to run into the issue of, you probably don't want to have your storage solution or this custom-built storage solution at the server level.
>- Your business logic which is effectively what your server is doing, should likely be separated out from your storage solution, probably you're gonna wanna have nice separation of duties in your system, and so that kind of falls apart.
> And so all that to say this is where a pub/sub pattern comes into play.

>- So the pub/sub pattern is the paradigm that consists of four entities.
>- The first entity is gonna be the publisher.
>- The second entity is gonna be the subscribers.
>- The third entity is what's called a topic.
>- Finally, the fourth entity is what's called a message.

> So what are these entities? what are their rules? What do they represent?
>- Well, the publishers are effectively gonna be the servers in the previous example of the chat application or the stock broker application.
>- And the servers, their job is to publish data to these topics.
>- You can think of the topics kind of like channels, conceptually speaking, they are channels of specific information.
```
       T1
P1 =========> S1

       T2
P2 =========> S2

       T3
P3 =========> S3
```

>- So here in topic 1 (T1) you might be publishing a specific type of data and in T2, you might be publishing a different type of data and so on and so forth.
>- Then the subscribers are gonna be the clients, that were originally listening for data from the servers, now these subscribers are gonna subscribe to topics.
>- So they are gonna be listening for data or for information from topics.

>- So taking a step back here, in the streaming example, we had our clients who were streaming directly from the servers.
>- But here with the pub/sub pattern, this is different. The subscribers do not communicate with the servers, they subscribe to topics and the publishers don't communicate with clients or with subscribers, they just publish data to topics.
>- So this is a very important concent in the pub/sub model.

>- It's the idea of the publishers and the subscribers don't really know about each other.
>- They just know about these topics.
>- The topics act as intermediary between the publishers and the subscribers.

> And then the fourth and final entity is messages.
>- These messages represent some form of data or some operation that is gonna be relevant to the subscribers and that the subscribers are basically gonna be listening for.
>- So the overarching flow is the publisher publishes data or rather publishes a message to a topic, the subscriber(s), subscribe to that topic, and as messages come into the topic, they are sent out to the subscribers that are subscribed to the topic.

> The message here, is not like a chat message. It refers to a data block. This could contain a chat message like a piece of text, but it could also represent an operation, to execute a stock trade, for example, or anything else. 
> So that is the pub/sub pattern in a nutshell.

>- These topics here that act as intermediaries between publishers and subscribers are effectively like a database solution.
>- All of the messages that are gonna be published to topics are going to effectively be stored in persistent storage in those topics, and what that means is that with a pub/sub system, you're guaranteed at-least-once delivery of the messages in a particular topic.
>- Every message that's sent or published to a topic is probably gonna keep track of some sort of index, or an ID representing all of the subscribers or each of the subscribers rather, that is listening to the topic, and when a message is pushed out to all of the subscribers, the subscribers are then likely going to acknowledge receipt of the message, it'll send back an ACK to the topic, and then the messages are gonna basically flip some sort of flag saying, oh, I've been consumed by subscriber one or I have been consumed by subscriber two, and that's sort of how it might work under the hood.

>- Now, one thing that's very important to note here, which is very much tied to the concept of at-least-once delivery being guaranteed, and the concept of persistent storage, which is the foundation of these topics, because you have these characteristics in a pub/sub system, what that means is that sometimes your messages might actually be sent more than once.
>- It is at-least-once delivery and not exactly-once delivery.
>- Exactly once delivery is something that's basically impossible to achieve in a distributed system. At least once delivery is possible, but what that means is that, you might encounter a situation where a message like M1 here gets pushed out to the subscribers, let's say to subscriber S1, but just as it gets pushed out, subscriber S1 maybe loses its connection to this topic. And what happens is S1 gets the message, but it doesn't send back an ACK to topic one. So subscriber S1 has received message one, but it isn't able to tell topic one that it has received message one.
>- And so what that means is that when subscriber one is eventually gonna reconnect to topic one or re-subscribe to it, message one in topic one is gonna realize that it hasn't been sent to subscriber one, or it'll think that it hasn't been received by subscriber one, and it might be sent a second time.
>- You see, this is why we have guaranteed at-least-once delivery, that message will be delivered to subscriber one at least once, but it might actually be delivered twice or three times, and this introduces a new concept that's very important to be aware of, when you're dealing with a pub/sub system.
>- It's the concept of an idempotent operation, or the concept of idempotency.
>- An idempotent operation is an operation that has the same ultimate outcome regardless of how many times it's performed.
>- So if a message gets delivered multiple times and it has an non-idempotent operation, that's gonna be bad for the system.
>- It's possible that even a non-idempotent operation might not be that bad. It's possible that you might be okay with a non-idempotent operation being performed multiple times.
>- But this is something to keep in mind because oftentimes you won't want to perform non-idempotent operations multiple times, and in those cases, a pub/sub system might have some drawbacks.

>- Now going back to the main characteristics of a pub/sub system, apart from the guaranteed at least once delivery of messages, which really stems from the persistent storage, the fact that these messages are stored in persistent storage, what's nice about a pub/sub system and about the topics is that they also give you ordering of messages. So as you send or publish messages to topics, they will be then pushed to your subscribers in the same order. So this is kind of like a queue.
>- And this is oftentimes very useful in a system if you're dealing with a chat application, you probably want chat messages to appear sequentially and in the order that they were sent.
>- If you are dealing with a stock broker application, and you're sending execution orders in your pub/sub system, you're probably gonna want these execution orders or these trade executions to be performed sequentially.
>- Or if you're sending stock prices to clients, you probably want those stock prices to appear sequentially in the order that you received them in at the publisher level.

>- So the ordering of messages is a very nice property of a pub/sub system.
>- And another really nice property of pub/sub systems that once again, stems from the underlying persistent storage is the fact that you can oftentimes replay messages in a pub/sub topic if you want to. There are a lot of pub/sub solutions out there that will give you this really nice characteristic or functionality of replayability or rewinding to a previous message, or to a previous snapshot in time of your topic, and that's something that can be useful sometimes, depending on the use case.

#### Why we have multiple topics ?
> The pub/sub system is effectively a database solution, a database that's got a bit of a different API than your typical database. It's also got this bi-directional concept to it. You've got subscribers, getting data from the database, and you've got publishers pushing data to the database. So it's a bit of a different concept than your normal database, but because this is effectively a database, you might be storing very different types of data in this database.
>- And so that's why it really makes sense to have multiple topics that might represent different types of data. They might not, you might be publishing to different topics, based on something completely different. Like, for instance, the location of the publishers, or the name of the publishers, etc., but you might also be publishing to different topics, just different types of data like you might be publishing stock prices to T1, and news alerts to T2.
>- And this ends up working in the favor of the systems designer or the systems administrator, because it's generally often really nice to have this ***clear separation of concerns and separation of duties*** even at the database level, or at the operations level.

>- Also, what's really nice with pub/sub systems is that you can then add stuff on to them. So for example, you can then add on content-based filtering at the subscriber level.
>- So you get the idea, you can basically add on more features or more functionality on top of a pub/sub system.
>- Also, there are a lot of very popular and very powerful pub/sub tools or pub/sub solutions out there, one very popular one is Apache Kafka. Another one is Google Cloud Pub/Sub, and these solutions often give you things out of the box.

>- So for example, Google Cloud Pub/Sub basically tells you that everything auto scales, because typically, you might have topics like T1, T2, T3, that themselves are sharded into different partitions.
>- Because this is a database solution ultimately, so T1 might actually be sharded into multiple shards.
>- But with something like Google Cloud Pub/Sub, you're basically told, don't worry about that. Your topics are just gonna scale automatically, you just have to think of T1, T2, T3, don't worry about sharding at the topic level, that's all taken care of, you don't even need to know about it.
>- Other things that might come out of the box like end-to-end encryption. A lot of these pub/sub offerings in the cloud, like in Google Cloud Platform, or AWS, will give you the ability to encrypt your messages such that over the network, they're encrypted, and then only subscribers know how to read them, you can make sure that messages only reach the relevant individuals, the people that you want to have received these messages so all that to say, there are really a lot of features, there's a lot of functionality that you can add to your pub/sub systems, or that come out of the box for free with the popular pub/sub offerings out there.

> And so all of these things, paired with the foundational characteristics of a pub/sub system or of the publish/subscribe pattern, all of these things put together, make the pub/sub pattern, an extremely powerful tool that you're really gonna want to have in your tool belt for systems design interviews.

---

### 23. MapReduce
> "MapReduce is a programming model for processing and generating big data sets with a parallel, distributed algorithm on a cluster."

#### 1 Prerequisite

- ***File System***
> An abstraction over a storage medium that defines how to manage data. While there exist many different types of file systems, most follow a hierarchical strutcure that consists of directories and files, like the **Unix file system**'s structure.

#### 3 Key Terms

- ***MapReduce***
> A popular framework for processing very large scale datasets in a distributed setting efficiently, quickly, and in a fault-tolerant manner. A MapReduce job is comprised of 3 main steps:
>	- the **Map** step, which runs a **map function** on the various chunks of the dataset and transforms these chunks into intermediate **key-value pairs**.
>	- the **Shuffle** step, which reorganizes the intermediate **key-value pairs** such that pairs of the same key are routed to the same machine in the final step.
>	- the **Reduce** step, which runs a **reduce function** on the newly shuffled **key-value pairs** and transforms them into more meaningful data.

> The canonical example of a MapReduce use case is counting the number of occurrences of words in a large text file.

> When dealing with a MapReduce library, engineers and/or systems administrators only need to worry about the map and reduce functions, as well as their inputs and outputs. All other concerns, including the parallelization of tasks and the fault-tolerance of the MapReduce job, are abstracted away and taken care of by the MapReduce implementation.

- ***Distributed File System***
> A Distributed File System is an abstraction over a (usually large) cluster of machines that allows them to act like one large file system. The two most popular implementations of DFS are the **Google File System** (GFS) and the **Hadoop Distributed File System** (HDFS).

> Typically, DFSs take care of the classic **availability** and **replication** guarantees that can be tricky to obtain in a distributed-system setting. The overarching idea is that files are split into chunks of a certain size (4MB or 64MB, for instance), and those chunks are sharded across a large cluster of machines. A central control plane is in charge of deciding where each chunk resides, routing reads to the right nodes, and handling communication between machines.

> Different DFS implementations have slightly different APIs and semantics, but they achieve the same common goal: extremely large-scale persistent storage.

- ***Hadoop***
> A popular, open-source framework that supports MapReduce jobs and many other kinds of data-processing pipelines. Its central component is **HDFS** (Hadoop Distributed File System), on top of which other technologies have been developed.
> Learn more: [https://hadoop.apache.org/](https://hadoop.apache.org/)

---

> As with many other systems design topics, MapReduce is pretty simple at face value, but it gets very complicated once you dive into its details.
>- The good news is that once again as with many other systems design topics, in the context of systems design interviews, what you need to know about MapReduce is actually relatively straightforward, relatively simple and it doesn't touch too much on those very complicated details.

> Now in order to fully understand what MapReduce really is, we have to go back in history all the way to the early 2000s when Google engineers were faced with a challenge, and the challenge that they were faced with was that they were dealing with very, very large data sets.
>- And as you might imagine, they had to process these data sets, and as you can imagine there's only so much vertical scaling that you can do when you're dealing with large data sets.
>- When you have a very large data sets, you eventually have to horizontally scale your system, you have to add machines to your system.
>- So these Google engineers had to process large data sets that were stored across hundreds if not thousands of machines.
>- Processing a data set that's stored across hundreds or thousands of machines is very difficult, it's a non-trivial task, you have to parallelize the processing across these hundreds or thousands of machines, you have to handle failures like network partitions or machine failures.
>- All of these things are difficult and these Google engineers had to figure out a way to process these large data sets in a distributed setting, efficiently, quickly and in a fault-tolerant manner, and so that's where MapReduce comes into play.

> In 2004 two very well-known Google engineers released a white paper on the MapReduce model, it was exactly that, it was a framework that allowed engineers or systems administrators to process very large data sets that were spread across hundreds or thousands of machines, so in a distributed setting, very efficiently, quickly and in a fault-tolerant manner.
>- Now the premise behind the MapReduce model, the premise that these engineers operated on was that the majority of data processing tasks could be split up or refactored so to speak into two steps; ***a Map step and a Reduce step***.
>- And these two steps of the Map and the Reduce were inspired by the Map and Reduce functions that a lot of functional programming languages have.
>- Now here in the context of MapReduce and in a distributed system setting, the Map and Reduce are a little bit different.
>- Those engineers created a library that would basically allow an engineer or a systems administrator to process huge data sets in the order of terabytes, spread across hundreds of thousands of machines very easily.

> So how did or how does this MapReduce model work?
>- Well, basically you've got your data and here we assume that we are in a distributed system, more specifically we have a distributed file system, in other words our data is stored across multiple machines.

>- The Map function is gonna transform the data into key value pairs.
>- And the fact that these are key value pairs is gonna be very important.
>- These key value pairs are gonna be the intermediate key value pairs because they live at the intermediate step in the entire MapReduce job or MapReduce process.
>- And then these key value pairs are gonna be shuffled around and reorganized in a way that makes sense, and here in the final step the Reduce step, they're gonna be reduced into some final output, and this output might be some file that you'll then use elsewhere in your system.

> And so at this point, as you can see, the concept of MapReduce is actually pretty simple.
>- You've got a data set that's spread across multiple machines you have some Map function that you, the engineer or systems administrator is gonna specify, that Map function is gonna transform your data set into intermediate values, the key value pairs, and then these key value pairs as for being reorganized in some way are gonna be reduced in some final step into some final output.

> **Few important points to note about MapReduce:**

1. >- The first one is that when we're dealing with a MapReduce model, we assume that we have a distributed file system, this means that we've got some large data set that is split up into chunks, these chunks are likely replicated and spread out across multiple machines in the order of hundreds or thousands of machines and then our distributed file system has some sort of central control plane that is aware of everything going on in the MapReduce job or process.
	>- What that means is that the central control plane knows where all of the chunks of data reside, it knows how to communicate with the various machines that store all of this data, it knows how to communicate with the machines that are gonna be performing the Map operations, you sometimes call them worker machines, same thing for the Reduce step, it knows how to communicate with the various reduce workers, it knows where your output is gonna live and so on and so forth.

2. >- The second thing that's important to note is that oftentimes because we're dealing with very large datasets, we don't actually want to move the large data set. We want to leave the data set wherever it resides, and what we do is we have the Map functions or the Map programs move to the data and operate on the data locally.
	>- So instead of grabbing all the data and maybe aggregating it and moving it elsewhere, we send the Map programs to the data, just in order to avoid moving all of this very large data.

3. >- The third thing that's very important to note about the MapReduce model, is that the key value pairs structure of the data that is in the intermediate step is very important.
	>- The reason it's important is because naturally when you perform a Reduce, when you reduce data values, especially data values that come from multiple chunks of the same data set, you're likely looking for some sort of commonality in these various pieces of data.
	>- Because when you've got key value pairs, then naturally you've got some keys that are gonna be common, and you can then aggregate them together and reduce them into one single meaningful value based on that key or relevant to that key.

4. >- Now the fourth thing that's very important to note about the MapReduce model is that one of the main things that this model ***tries to accomplish is to handle faults, to handle failures***.
	>- Like for instance, if there's a network partition or a machine failure.
	>- In order to handle machine failures, what a MapReduce job is gonna do is it's basically just gonna re-perform a Map operation or Reduce operation where a failure occurred.
	>- Now what that assumes is that our Map function is idempotent that's really important.
	>- When we're talking about the MapReduce model, we almost always assume or rather we almost always require that the Map function and that the Reduce function be idempotent, in other words if we repeat a Map function or Reduce function multiple time, we need the outcome to be the same regardless of how many times we've repeated that Map function or that Reduce function.
	>- So that's really important the idempotency of your Map and Reduce functions.

5. >- And then the final point that's very important to note about the MapReduce model is that as the engineer or the systems administrator who's dealing with a MapReduce job, the main thing that you care about is what Map function you're gonna specify, what Reduce function you're gonna specify, and what the various inputs and outputs of those functions is gonna be, that's really all you care about.

> So as you can see this framework simplifies a lot of things for engineers, that just means that engineers have to worry about what the various inputs and outputs of their data is gonna be, which is what they were concerned with in the first place when they thought of processing a data set and that's it.
>- They don't have to worry about all of the intricacies of processing a data set in a distributed system, because that's when the MapReduce framework or rather the MapReduce library at this point.

> And as you can probably imagine this MapReduce model can be applied to all sorts of problems.
>- Like for example, imagine you had a bunch of YouTube videos stored in some data set and you had metadata about those YouTube videos, and you wanted to get maybe the total number of views or of likes per user or per YouTube channel.
>- You might use a MapReduce job to get that data from that huge data set of YouTube videos.
>- Or maybe imagine if you had some huge data set of logs in your system, so imagine you had a bunch of logs from various services in your system like logs from your payment service, logs from your authentication service and you wanted to maybe count the total number of logs per service, or the total number of logs in some interval of time. You might use a MapReduce job to accomplish just that.

> There are so many data processing tasks that can be expressed in the MapReduce model.

> So this is what MapReduce is, it's an incredibly useful concept or framework when you're processing large datasets in a distributed setting and it's definitely gonna be a tool that you're gonna want in your tool belt when you jump into a systems design interview.

---

### 24. Security And HTTPS
> While network security is of critical importance to virtually any system, it's beyond the scope of most system design interviews.

> That being said, having even a cursory understanding of a few key concepts could very well materialize into the edge you need to ace your interview and secure--pun perhaps intended--a job offer.

#### 9 Key Terms

- ***Man-In-The-Middle Attack***
> An attack in which the attacker intercepts a line of communication that is thought to be private by its two communicating parties.

> If a malicious actor intercepted and mutated an IP packet on its way from a client to a server, that would be a man-in-the-middle attack.

> MITM attacks are the primary threat that encryption and **HTTPS** aim to defend against.

- ***Symmetric Encryption***
> A type of encryption that relies on only a single key to both encrypt and decrypt data. The key must be known to all parties involved in communication and must therefore typically be shared between the parties at one point or another.

> Symmetric-key algorithms tend to be faster than their asymmetric counterparts.

> The most widely used symmetric-key algorithms are part of the Advanced Encryption Standard (**AES**).

- ***Asymmetric Encryption***
> Also known as public-key encryption, asymmetric encryption relies on two keys--a public key and a private key--to encrypt and decrypt data. The keys are generated using cryptographic algorithms and are mathematically connected such that data encrypted with the public key can only be decrypted with the private key.

> While the private key must be kept secure to maintain the fidelity of this encryption paradigm, the public keyy can be openly shared.

> Asymmetric-key algorithms tend to be slower than their symmetric counterparts.

- ***AES***
> Stands for **Advanced Encryption Standard**. AES is a widely used encryption standard that has three symmetric-key algorithms (AES-128, AES-192, and AES-256).

> Of note, AES is considered to be the "gold standard" in encryption and is even used by the U.S. National Securty Agency to encrypt top secret information.

- ***HTTPS***
> The **H**yper**T**ext **T**ransfer **P**rotocol **S**ecure is an extension of **HTTP** that's used for secure communication online. It requires servers to have trusted certificates (usually **SSL certificates**) and uses the Transport Layer Security (**TLS**), a security protocol built on top of **TCP**, to encrypt data communicated between a client and a server.

- ***TLS***
> The **T**ransport **L**ayer **S**ecurity is a security protocol over which **HTTP** runs in order to achieve secure communication online. "HTTP over TLS" is also known as **HTTPS**.

- ***SSL Certificate***
> A digital certificate granted to a server by a **certificate authority**. Contains the server's public key, to be used as part of the **TLS handshake** process in an **HTTPS** connection.

> An SSL certificate effectively confirms that a public key belongs to the server claiming it belongs to them. SSL certificates are a crucial defense against **man-in-the-middle attacks**.

- ***Certificate Authority***
> A trusted entity that signs digital certificates--namely, SSL certificates that are relied on in **HTTPS** connections.

- ***TLS Handshake***
> The process through which a client and a server communicating over **HTTPS** exchange encryption-related information and establish a secure communication. The typical steps in a TLS handshake are roughly as follows:
>- The client sends a **client hello**, a string of random bytes to the server.
>- The server responds with a **server hello**, another string of random bytes as well as its **SSL certificate**, which contains its **public key**.
>- The client verifies that the certificate was issued by a **certificate authority** and sends a **premaster secret**, yet another string of random bytes, this time encrypted with the server's public key to the server.
>- The client and the server use the client hello, the server hello, and the premaster secret to then generate the same **symmetric-encryption** session keys, to be used to encrypt and decrypt all data communicated during the remainder of the connection.

---

#### 1st Disclaimer
> Security is one of those concepts that you don't actually quite need in a systems design interview.
>- In other words, whereas these other concepts you're almost certainly gonna run into in a systems design interview, and you are gonna be expected to know them.
>- Security you are unlikely to run into in a systems design interview.
>- And you're almost certainly not going to be expected to know that much about security.
>- That being said, it is very good to be familiar with security at a high level at least.
>- Because, as you know, systems design interviews can go in many different directions.
>- And it's very possible that depending on your systems design interview, you might start having a conversation with your interviewer that leads into some topic about security or something related to security.
>- And if you're familiar with security, if you have a decent understanding of the building blocks of security, then you will be ahead of the game.
>- It will be objectively better for you to have that knowledge.
>- So you can treat security kind of like a bonus topic.
>- That's really good for you to know but that's not something that you should stress too much about.

#### 2nd Disclaimer
> Security is one of those fields where you're typically either an expert or someone who actually doesn't really know much about the field.
> Because it's just a very domain expertise, heavy type of field and a very complicated type of field.

> Let's jump into the topic of security and HTTPS.
>- In the modern day and age in modern day systems, most machines communicate with one another over HTTP.
>- HTTP is a communications protocol that offers an abstraction over or on top of TCP.
>- It's really nice for developers because it's much more easy to manipulate and to kind of extend and it's basically what the internet runs on.
>- So when you've got a client interacting with a server online they usually do so over HTTP.

>- Now speaking of a client interacting or communicating with a server online over HTTP, when we think of that, when we think of that communication or interaction, there's this implied assumption of privacy.
>- In other words, you would expect that any message that's sent from a client to a server over HTTP or from a server to a client over HTTP would be private between the two parties communicating between the client and the server.
>- That's just something that you probably assume because you just think that, hey, if you've got two parties communicating just with one another, their communication should be private.
>- We obviously want it to be private, because they might be exchanging sensitive information. And so that's what we assume.

> But that would actually be an incorrect assumption.
>- Because it turns out that when you've got two machines, let's say a client and a server communicating over HTTP, a malicious actor who is well trained or who has access to the correct tools, can actually hijack this communications channel between the client and the server.
>- Can intercept the underlying IP packets that are being transferred between the client and the server.
>- And can either eavesdrop on them by just reading them and not telling anybody, which is really bad.
>- If we're talking about private information, even information that's not particularly private.
>- Again, there's this assumption that a communication between two parties should be private.
>- So a malicious actor could intercept an IP packet or a set of IP packets could read the messages or the data and those IP packets could even alter them and relay them to either the server or the client in an alternate fashion.
>- In any case, this is obviously bad.
>- This is a breach of privacy or security, whatever you wanna call it.

> Some third party, basically intercepting a communication between two other parties that is expected to be private or that the two other parties don't realize is being breached.
> This is known as a man-in-the-middle attack.

>- It is a well known occurrence in the field of security, which is why it's got a name.
>- And sometimes you'll see it written by its acronym MITM attack, man-in-the-middle attack.
>- And so this is really at the core of what we're trying to solve with security.
>- We're trying to prevent a man-in-the-middle attack or not necessarily prevent a man-in-the-middle attack, but prevent the consequences of a man in the middle attack.
>- Namely, the consequences of having an unwanted third party read on our communication between a client and a server.
>- Communication that we want to be private, communication that we want to be secure.

> So HTTPS is gonna be the same as HTTP, except it's gonna have secure after it. We're gonna have to figure out, why is it secure? Or rather, how is it secure?
> Because clearly right now, when you've got a client and a server communicating over HTTP, their communication is anything but secure.

> Encryption is gonna be a key component to the secure aspect of HTTPS.
>- So encryption, let's say that we've got our client communicating with our server.
>- And the client is sending a message to the server that it wants to be private.
>- Let's say that the client is sending a simple string, just the string hello to the server.
>- But it obviously doesn't want anybody except for the server to be able to read that message.
>- Naturally, you would want to somehow hide that message or obfuscate that message.
>- And that's where encryption comes into play.

> The idea behind encryption is that you can somehow encrypt a message, meaning you turn it into a random string of characters or a seemingly random string of characters something that is illegible.
>- And this isn't even necessarily a string of characters. It's simply any form of the data that is no longer legible that cannot be tied back to the original data at least at first once.
>- And then that encrypted data should be able to be decrypted by a particular party.
>- So in this case, it would be the server.
>- So again, the idea behind encryption is you've got a message let's say hello. you encrypt it somehow into some random piece of data or string of characters that nobody can really understand.
>- And then the server can decrypt that random message somehow.
>- And decrypting it will return the original underlying message, hello.

> Now here we're gonna talk about two primary families or systems of encryption, called symmetric encryption and asymmetric encryption.
> And here mini disclaimer that this is where we're gonna start to really just talk about this at a high level because this part of security encryption gets very complicated very fast and it's very math heavy, we're not gonna get into that.

> But so from a high level, what is symmetric encryption? What is asymmetric encryption?
>- Symmetric encryption is a type of encryption that relies on symmetric key algorithms.
>- Symmetric key algorithms are a type of cryptographic algorithm that relies on a single key.
>- And a key might be a special string, a single key to both encrypt and decrypt data.

>- So for example, imagine I've got a key which is the string foobar, I can use a special symmetric key algorithm to encrypt a message to encrypt some data using that key foobar.
>- And the only way that data or rather that that encrypted data can be decrypted is using that same key foobar.
>- And in practice, symmetric encryption usually uses something called AES, Advanced Encryption Standard.
>- And AES is basically a specification of encryption and it uses or describes a symmetric key algorithm that uses or relies on a single key to both encrypt and decrypt data.

> And one really nice thing about symmetric encryption is that it's very, very fast.
>- It's very fast to both encrypt and decrypt messages.
>- In fact, it's faster than its asymmetric counterpart.
>- Because it relies on only one key, that one key has to be shared between the two parties that are communicating.
>- And while that might be fine, in certain cases like for example, imagine that you had a friend, and you wanted to communicate by email using symmetric encryption, you can maybe decide on a key in person, tell your friend the key out loud, only you two have ever heard the key, and then you use that key to encrypt and decrypt messages by email.
>- That would be fine, no one else would be able to find that key.

> But now if we go back to systems design, let's say that we're dealing with a client and a server communicating with one another over the network.
>- How do the client and the server establish a common key? That key will have to be shared between them.
>- And in order to be shared, you need it to be shared over a security communications channel.
>- Otherwise, you're still vulnerable to a man-in-the-middle attack.
>- Because for example, you could say, okay, when a client, let's say a browser connects to a website server, the very first thing that the server does is give the client some key that they can use for symmetric encryption.
>- Okay, great. But what if there's a malicious actor in the middle that intercepts that message, grabs the key and can now decrypt any encrypted message, you're left with the same problem.
>- So clearly symmetric encryption, while really nice alone doesn't actually solve our HTTP vulnerability.

> So now let's talk about asymmetric encryption.
>- Asymmetric encryption, which is also known as public key encryption is a different type of encryption where instead of relying on a single key to encrypt and decrypt messages, you rely on two keys to encrypt and decrypt messages.
>- Specifically, you have a pair of keys that are generated together. We call one of them the public key, and the other one, the private key.
>- And so these two keys or this pair of keys is generated mathematically using some cryptographic algorithms.
>- And they are mathematically bound, such that if you encrypt a message using the public key, that message can only be decrypted using the private key.
>- These are really complex algorithms, complex math, but that's the key point to remember.
>- That any message which is encrypted using the public key of a public private key pair that's been generated mathematically, any such message can only be decrypted using the private key.
>- And as the names public and private suggest, if you're an entity, let's say you're a server, and you own a public private key pair, you will make the public key publicly available. So anybody can see your public key.
>- And presumably, anybody can encrypt messages using that public key. But then the only person who has access to the private key is you or is the server in this case.
>- So the server would be the only person or the only entity who is able to decrypt messages that have been encrypted using the publicly available public key because the server is the only entity that has access to the private key.
>- So asymmetric encryption is very interesting, quite a bit different from symmetric encryption because it relies on two keys rather than one.
>- And also, it's slower than symmetric encryption.

> But so this all brings us to HTTPS, which is really the main thing that we're interested in here. How do we make HTTP secure?
>- Okay, so HTTPS is an extension of HTTP that runs on top of something called TLS.
>- TLS stands for Transport Layer Security. And TLS is basically a security protocol.
>- Which is why by the way, sometimes you'll hear HTTPS referred to as HTTP on top of TLS. Or another way to word it is that with HTTPS communication is encrypted using TLS.
>- And by the way, it turns out that the predecessor protocol to TLS was something called SSL, which stands for Secure Sockets Layer.

> SSL certificates are certificates that are granted by a trusted third party called a certificate authority.
>- This is a trusted third party that we as a collective humanity, or rather developers has agreed to trust.
>- This might be a nonprofit organization or even a for profit organization. But the point is, they are trustworthy.
>- And they will give out these SSL certificates to parties like algo expert, for example.
>- So the algo expert servers will have the algo expert SSL certificate.
>- And the certificate is basically a digital item that a certificate authority a trusted third party has signed and that serves to assure the client that is gonna rely on the certificate that the server is who they say they are.

> And this is how HTTPS works.
> This is how modern day systems can have security or at least security in their communication.

---

### 25. API Design

#### 1 Prerequisite

- ***ACL***
> Short for Access-Control List. This term is often used to refer to a permissioning model: which users in a system can perform which operations. For instance, APIs often come with ACLs defining which users can delete, edit, or view certain entities.

#### 2 Key Terms

- ***Pagination***
> When a network request potentially warrants a really large response, the relevant API might be designed to return only a single **page** of that response (i.e., a limited portion of the response), accompanied by an identifier or token for the client to request the next page if desired.

> Pagination is often used when designing **List** endpoints. For instance, an endpoint to list videos on the YouTube Trending page could return a huge list of videos. This wouldn't perform very well on mobile devices due to the lower network speeds and simply wouldn't be optimal, since most users will only ever scroll through the first ten or twenty videos. So, the API could be designed to respond with only the first few videos of that list; in this case, we would say that the API response is **paginated**.

- ***CRUD Operations***
> Stands for **Create, Read, Update, Delete** Operations. These four operations often serve as the bedrock of a functioning system and therefore find themselves at the core of many APIs. The term **CRUD** is very likely to come up during an API-design interview.

---

> ***API design is distinct from systems design.***
> ***Specifically, API design is not a subset of systems design, but instead it's a sibling of systems design.***

> In fact, if you interview at a big tech company or at a tech startup, you will usually in a set of technical interviews, be given either a systems design interview or an API design interview.
>- This sort of confirms the idea that API design is a sibling of systems design and not a subset of systems design.
>- It's important to understand why API design interviews even exist.

> Systems design is so important because when you've got a software product or service that you are building, especially at scale, the system that is going to enable that product or service is going to be very complex and it's important to be able to design it well.

> *But what about APIs? Are APIs all that important? Is designing an API all that important? - YES**
>- In order to understand that you can just think of any product or service out there, specifically a software based product or service, and you'll quickly realize that there is an API that backs that product or service.
>- If you think of YouTube, Twitter, Facebook AlgoExpert, the very website that you're on right now for all of these software products and services there is an API that backs them. There might even be multiple APIs that back of them.
>- But the point is there is at least one API, and it really is at the core of the product or service because without that API you just wouldn't have most of the functionality for all of these products and taking it a step even further there are some software products or services like Stripe, for example.
>	- Stripe is a company that provides a payments processing solution for businesses.
>	- And one of their core products, is effectively an API.
>	- So their actual product is the API. It's not even like the API backs their product. Their product is the API.
>	- Of course, they also have auxiliary products, they have dashboards, all sorts of things, but the point is some products and services literally sell access to an API.
>- So APIs are extremely important and now if we talk about designing APIs, obviously if APIs are this important then designing them well is gonna be really important, but something that's really worth noting here is that when you are dealing with an API, there is a sense of permanence to it.
>- Let's say that you develop an API and you release it to the world and suddenly you've got customers who are using that API, be they external customers, people outside of your company, or perhaps engineers within your company who are consuming your API, or maybe other products and services that are integrating with your API and consuming it, relying on it for their operations, as soon as that happens, making changes to your API or removing parts of your API, removing your API altogether all of these things become extremely difficult if not impossible, just because you have so many people, so many products and services relying on your API, and that makes designing an API all the more important.
>- It means that any design decision in your API, even the most seemingly trivial detail like the name of a parameter in an endpoint or the ordering of parameters in an endpoint, all of these minor details become extremely important because suddenly they're gonna have long lasting consequences on a lot of people, and a lot of other products and services and that's why a big tech companies like Google for example, when a new API is being developed by some team at Google, that API goes through a very rigorous not only design process but also review process where you've got typically very high level engineers, external to the team that's developing the API, who review that API, who review the design choices, really dissect the API, challenge every little detail that you could think about the API and it's just a very long process, which goes to show you just how important API design is.

> So the main way in which these two genres (*Systems design and API design*) of interviews are similar is in the way that the first 10 minutes of an interview in both genres goes.
>- Imagine that you had a systems design interview at some company, you might be asked to design Twitter, or to design Stripe.
>- And then as the interviewee you would have to ask a lot of clarifying questions.
>- You would have to disambiguate the problem statement, really ask what part of Twitter are we designing? What part of Stripe are we designing?
>- You know, what functionality do we really want to support?
>- And then of course you would ask a few questions about maybe the scale of the system, maybe what regions we're gonna be supporting, et cetera.

> Well, equivalent API design interview questions would probably be something like design the Twitter API, or design the Stripe API, similarly ambiguous, similarly vague and you would still have to as the interviewee ask a lot of clarifying questions like, well, what part of Twitter are we designing this API for? What part of Stripe?
>- Are we just designing the API that supports the functionality on the home page of Twitter?
>- Is it for the trending tab? Is it for the settings tab? Who's gonna be consuming our API?
>- So you see, you're asking very similar questions and you're really trying to get a lot more information that you can use to then actually design this API.
>- Because without this information you can't properly design this API, you don't really know what you're about to do.

>- And then once this introduction is over, once you've gotten all information that you need, then you jump into the meat of the interview and here the two interviews start to diverge a lot. They look quite a bit different, but they still share a few similarities.

> In a systems design interview this is when you would probably start to draw out some diagrams, talk about the various systems components.
> Maybe you would write out things like, you know, what a SQL table looks like if you're relying on a SQL table for storage, but that's generally the gist of the systems design interview.

> The API design interview is gonna look a lot different. You're not really gonna be drawing out diagrams.
>- You're not at all gonna be relying on systems designed components.
>- Instead, what you'll be doing is you will be writing an outline of sorts of the API.
>- So you're likely gonna be writing out the various entities or resources that this API is gonna rely on.
>- So for example, if we're talking about Twitter, there would likely be a tweet resource or entity.
>- If we're talking about Stripe, there would likely be a charge or payment resource or entity, a customer entity, and you would write out what these resources or entities look like, what properties or attributes they have.
>- Then you would write out an outline for the various API end points that your API needs to have.
>- You would write out the various parameters that the API end points take, the various responses that the API end points return.
>- But what you wouldn't do is you wouldn't write out any logic.
>- You wouldn't be actually implementing the API end points, just outlining them.

> ***This is where the two genres (Systems design and API design) of interviews diverge but they do still share the similarity of there isn't really a right or wrong answer in an API design interview or in a systems design interview. Obviously this is within reason.***

> For example, if you're in a systems design interview and you tell your interviewer that you're gonna store, you know, all historical messages or posts on Twitter in memory, on a single server, that's probably not gonna be like an acceptable solution.
>- Your ***systems design choices need to actually be sound***.
>- They ***need to be backed by logic or arguments***.
>- You **need to be able to defend them properly**.

> But ***otherwise, if you can defend*** your decision for some systems design choice, ***then anything is kind of fair game***.

> Similarly for API design not every API is gonna look the same.
>- What one interviewee might give for a design for a particular API might look very different from what another interviewee might give.
>- And both of them might be defensible.
>- Both of them might be sound so long as you can actually explain why you're doing things and there isn't really a right or wrong answer.
>- ***This is much more about having a conversation with your interviewer, telling them why you're making certain decisions, being open to their feedback and their criticism just as you would be if you were say at Google developing an API and an API reviewer came to you and gave you a bunch of criticism, constructive criticism, you would probably have a conversation with them, maybe a little bit of a debate around why you made certain choices.***
>- Well, that's what we're looking for in an API design interview.

> Mostly in an API design interview, just the outline of an API is expected.
>- Very simple, very straightforward, not necessarily easy, right?
>- This is still a lot of stuff to come up with and to design in a 45 minute interview, or let's say even 35 minutes, if you've spent 10 minutes kind of disambiguating the problem statement, but it isn't too complicated.
>- It's not like there is too much to do.
>- Now depending on your preferences and your background, what you're used to, if you've designed APIs in the past, you might want to write out your API outline in a different format such as Swagger.

>- [Swagger](https://swagger.io/), I suppose is the official way to define APIs.
>- It is an interface description launguage.
>- It's a format to describe APIs.

> But so if you are someone who's used to swagger, for example, or if you like things being a little bit more verbose and it helps you better organize your thoughts, then this type of format might be good.
>- At the end of the day the key thing is whatever you're most comfortable with and whatever your interviewer is okay with.
>- So you would likely ask them, is it okay if I just go with this approach?

> ***But so all in all, this is what you can expect to deliver in an API design interview.***

#### Few publicly available API documentations
- [Stripe API](https://stripe.com/docs/api)
- [Twitter API](https://developer.twitter.com/en/docs/twitter-api/getting-started/about-twitter-api)

---
