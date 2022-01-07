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
> Short for **Domain Name System**, it describes the entities and protocols involved in the translation from domain names to IP Addresses. Typically, machines make a DNS query to a well known entity which is responsible for returning the IP address (or multiple ones) of the requested domain name in the response.

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
  >- a **payload**, which isi just the data being sent over the network.
