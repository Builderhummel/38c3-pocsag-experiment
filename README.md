# Introduction
We are conducting an experiment during the congress to test out the capabilities of our self-built POCSAG transmitter. We try to answer the following research question:

**RQ1:** Is the transmitter suitable to handle a large congress?

# Experimental Setup
The transmitter is strategically placed at the 38c3. The main goal is to cover as much of the venue area with the transmitter as possible. We use the frequency **439.9875MHz** (*standard amateur radio POCSAG frequency*).

To increase the amount of test devices, we distribute self constructed pagers to visitors at 38c3. They are tasked to document their receptions.

To obtain a realistic setup, we will use organic test data. We are generating this data using the input of 38c3 visitors. It can be obtained through various ways (direct, telegram, etc.)

# How to help us with the experiment
Any help with the experiment is welcome. You can support us in 2 ways:
1) Generate messages to increase the load of the transmitter
2) Receive messages sent by the transmitter and provide us with a report of your observations

## How to generate messages
There are multiple ways to convey the messages to us, so we can use them as organic traffic samples to increase the load of the transmitter.

### By phone
To convey a message via phone, you can call our hotline -7300.

Please provide the following information
- Message Content
- RIC (optional; will default to **1111**)

### By Telegram (the paper)
The Chaoswelle assembly kindly supports us in executing our experiment. You can pay them a visit at their assembly and fill out the paper sheet. 

Please provide the following information
- Message Content
- RIC (*optional*; will default to **1111**)
- (Nick-)Name (*optional*)

### By paying us a visit at our assembly (Signalspielplatz)
Of course you can also visit us at our assembly. Just ask a member nicely and they will take your message.

## How to create reception reports
To create a reception report, you can bring your own receiver (Pager, SDR, FSK Boards, etc). The reception of amateur radio transmissions is allowed in Germany by licensed and non-licensed people.

A RIC is a series of bits included in every message to tag them. This tag can be used to filter out messages of interest. To obtain the maximum amount of data, we *recommend* to set the RIC to wildcard to receive every message transmitted.

The following table displays a possible RIC filtering suggestion for real life applications:
- **xxxxx** - RIC with 5 figures (e.g. **69420**)
- **8** - RIC for transmitter info
- **1111** - General Messages
- **1142** - Upcoming talks

The callsign of the transmitter is transmitted using the RIC **8**. Every organic message conveyed to us without a specific RIC defaults to **1111**.

### Information contained in the reception report
To inform us about your results in receiving our transmitter, we would kindly ask you to provide the following information:
- Position (e.g. Hall 1, Toilet T11, 2nd floor main hall near assembly xyz, etc.)
- RIC of received message
- Message content (*optional; partial receptions are also interesting to us*)
- Signal strength (*optional*)

To convey these information, just pay us a visit at our assembly. Hand-in by paper is preferred. We can provide you a sheet of paper.

#### QSL Cards
Everyone who is providing a reception report according to our standards is eligible to receive a QSL-Card. We will hand them out for free :-) (*limited supply*)

# Borrow a free pager (and bring it back afterwards)
We are aware that the least amount of visitors will bring their own pager. To support our experiment, we constructed a pager based on ESP32 and SX1278.

You can borrow one for free for up to **6h**. After this time period your are **REQUIRED** to bring it back to our assembly. (*We only have a very limited amount of them and there are more people interested than pagers available*)

You have to provide the following data when borrowing one:
- Name
- Matrix Handle
- Planned return time

This data will be immediately (permanently) deleted after you brought us the pager back.

While we provide the pager, you have to supply the following equipment:
- USB C cable
- Powersource (e.g. Smartphone, Powerbank *(be aware that our pager is very power efficient. Some Powerbanks will turn off automatically after some time)*)

## Call for code
If you are interested in embedded programming and want to support us with the firmware, feel free to contribute. During the development and testing time, you can exceed the **6h** period (we can also discuss an acquision - lets have a chat about this :)).

[Pager Firmware on Github](https://github.com/Numbernaut/ESP32-POCSAC-Reciever)
