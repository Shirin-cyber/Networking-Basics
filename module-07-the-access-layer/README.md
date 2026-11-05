# Module 7: The Access Layer

> Networking Basics · Cisco Networking Academy

---

## 7.0 Introduction

### 7.0.1 Why should I take this module?

It's lunch break, and Kishori runs into her friend **Rina**, who works as an **IT support technician** at the hospital. They decide to eat together, and Kishori figures this is a good chance to ask something she's been wondering about.

Here's what she knows now:

- Her desktop at the nurses' station connects to the network with a **twisted-pair cable**.
- Most of her other devices connect **wirelessly**.

So her question is: **is there any difference in how wired and wireless devices communicate on the network?**

Rina knows Kishori has relatives in the **United States**, so she explains it like this: the difference between wired and wireless communication is similar to the difference in **addressing formats when mailing packages to different countries**. The **contents inside** might be exactly the same, but the **addressing and maybe the packaging** can be very different.

Then the module asks the big question: **how does a message get delivered?**

When I write a letter and put it in an envelope, I have to put the right **address** on it so it reaches the recipient. In a network, **placing one message format (the letter) inside another message format (the envelope)** is called **encapsulation**.

**Connecting the dots:**

- Remember my guess in Module 6 that Kishori's desktop was on a **UTP cable**? Turns out that's right. Rina's story confirms it.
- **Encapsulation** came up in 5.1.2, where each message needs a **header with addressing info**. Now the course gives me a way to picture it: the letter is the **data**, and the envelope is the **header** with the address on it.
- The "packages to different countries" idea makes sense to me like this: the message is the same whether it goes over a cable or over Wi-Fi, but the way it's **wrapped and addressed** depends on the type of connection.
- In 5.3.4, the **data link layer** was where **frames** get exchanged. This module's topic has "**Ethernet frame**" in the title, so I think this is where that gets explained.

---

### 7.0.2 What will I learn in this module?

**Module title:** The Access Layer

**Module objective:** Explain how communication occurs on Ethernet networks

Here's what's in it:

| Topic | What I'll be able to do |
|---|---|
| **Encapsulation and the Ethernet frame** | Explain the process of encapsulation and Ethernet framing |
| **The access layer** | Explain how to improve network communication at the access layer |

A few thoughts before I start:

- **Encapsulation and the Ethernet frame** is probably about how a message gets wrapped up, and what the **frame** looks like when it travels on an Ethernet network. I'm guessing the **MAC address** and **NIC** from 5.2.1 show up here, since the video said they'd be explained later.
- **The access layer** sounds like it's connected to the **network access layer** from the TCP/IP model in 5.3, which is where Ethernet lives. The objective is about **improving** network communication, so I'm guessing it covers how devices like switches help.
- This module also matches one of the goals from the course intro: **explain how communication occurs on Ethernet networks**.
