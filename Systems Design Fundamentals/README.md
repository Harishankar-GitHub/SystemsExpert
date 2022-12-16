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
