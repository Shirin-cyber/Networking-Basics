# 1.3 Bandwidth and Throughput

> Module 1: Communications in a Connected World
> **Topic objective:** Explain network transmission speed and capacity

---

## 1.3.1 Bandwidth

Think about streaming a movie or playing a multiplayer game. Both need a connection that's fast and reliable. Apps like these are called **high bandwidth** applications, and to support them the network has to send and receive bits at a really high rate.

Different physical media (remember copper, fiber, and wireless from 1.2?) can move bits at different speeds. People usually talk about that speed using two words: **bandwidth** and **throughput**. I'll deal with bandwidth first.

**Bandwidth = the capacity of a medium to carry data.**

More specifically, digital bandwidth is how much data can flow from one place to another in a given amount of time. It's measured in **bits per second**, and the key word is that this is what can *theoretically* be sent. So it's the maximum, not necessarily what I'll actually get. (I'll come back to that in throughput.)

What decides how much bandwidth is available? Three things: the **properties of the physical media**, the **current technology**, and the **laws of physics**. So there's a real limit to how fast something can go.

### Units of bandwidth

| Unit | Stands for | Equals |
|---|---|---|
| **bps** | bits per second | 1 bps (the basic unit) |
| **Kbps** | thousands of bits per second | 1 Kbps = 1,000 bps |
| **Mbps** | millions of bits per second | 1 Mbps = 1,000,000 bps |
| **Gbps** | billions of bits per second | 1 Gbps = 1,000,000,000 bps |
| **Tbps** | trillions of bits per second | 1 Tbps = 1,000,000,000,000 bps |

**Connecting the dots:** this is all in **bits**, not bytes. From 1.2, a byte is 8 bits, so a small "b" and a big "B" are not the same thing. I think that means a connection of 8 Mbps moves roughly 1 megabyte per second. Good to keep in mind when I'm looking at internet plans or download speeds.

---

## 1.3.2 Throughput

Throughput is also a measure of how many bits get across the media in a certain amount of time. So it sounds the same as bandwidth, but there's a catch: **throughput usually doesn't match the bandwidth.**

So my guess from the Module 1 intro was right. They're related but not identical:

- **Bandwidth** = what the connection *can* do in theory (the capacity)
- **Throughput** = what actually happens in real life

An easy way for me to picture it: bandwidth is how many lanes a road has, and throughput is how many cars actually get through once you add traffic, accidents, and slow spots.

### What affects throughput?

- **The amount of data** being sent and received over the connection
- **The types of data** being sent
- **Latency** caused by how many network devices the data runs into between the source and the destination

**Latency** = the time it takes for data to get from one point to another, including any delays along the way.

### A couple of other things that stood out

**1. Throughput counts every bit, useful or not.**
It doesn't care whether the bits are valid or useful to me. A lot of the messages on a network aren't meant for any app I'm using. For example, there are network control messages that regulate traffic and correct errors. They still take up space, so they still count toward throughput.

**2. The slowest link wins.**
In a network with multiple segments (like an internetwork), throughput can't be faster than the **slowest link** on the path from the sender to the receiver. Even if almost every segment is super fast, one slower segment slows down the whole thing.

It's like a chain: it's only as strong as its weakest link, except here it's speed instead of strength.

There are plenty of online speed tests that can show the throughput of an internet connection.

---

## 1.3.3 Video: Throughput

This video shows throughput using **speedtest.net**, though there are other sites that do the same kind of thing.

**Throughput** = the amount of data sent and received over a connection, **including any delays**, in both directions. Delays can happen sending messages out or receiving them coming in.

### What happens in the test

1. Click **Begin Test**.
2. The site downloads some messages, and the **download speed** shows up. That's the number of bits per second being *received*. It's measured in **megabits per second (Mbps)**, which is millions of bits per second.
3. Then it measures the **upload speed**, the bits per second being *sent*.

### The numbers from the video

| | Speed |
|---|---|
| **Download** | 35.70 Mbps |
| **Upload** | about 35 Mbps (the transcript says both 35.04 and 34.04, so I'm going with "about 35") |

Download came out slightly higher than upload. The video says that's typical at home: you can usually **receive** data faster than you can **send** it.

**Connecting the dots:** the video calls these numbers the "bandwidth," but the reading just said speed tests show **throughput**. I think it makes sense because the test measures what actually gets through on my connection *right now*, delays and all, and that's throughput. It's a good way to check how close my connection is to what's promised.

These tests don't only show how my own network is doing. They also show how my **internet service provider (ISP)** connection is performing. I'd like to try one on my own Wi-Fi at some point.

---

## What I want to remember

- **Bandwidth** = the capacity of a medium to carry data, measured in bits per second (bps, Kbps, Mbps, Gbps, Tbps). It's the theoretical max.
- **Throughput** = how much data actually gets across in a given time, including delays. It's usually lower than bandwidth.
- **Latency** = the time it takes for data to travel from one point to another, including delays.
- Throughput is affected by the amount of data, the types of data, and the number of devices between source and destination.
- **The slowest link** in the path limits the throughput of the whole network.
- Speed tests (like speedtest.net) measure throughput. Home connections usually have higher download than upload.
