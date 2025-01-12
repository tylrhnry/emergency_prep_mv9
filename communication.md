# Communication
Communication is arguably the most important subject when dealing with emergencies. It is also very susceptible to degradation.

## How we do things now
The primary ways we currently communicate are
- In-person
- Cellular (text and calls)
- Internet-based, federated protocol (email)
- Internet-based, centralized app (Slack, Circles, Facebook)
- (Radio)

Each of these methods has pro's and con's, and it is generally good to have multiple of these methods established.


## In-person
In-person communication tends to be fairly resilient and effective, but generally requires proximity, pre-established plans to meet, and the same time availability. It can also be highly dependent on travel conditions. Extreme weather, civil unrest, and health concerns (like disease outbreak) are the main disruptors of in-person communication. Other than the natural limitations of needing to be in the same place at the same time, in-person communication is very resilient.


## Cellular
Text and phone calls offer much more flexibility with location and time requirements. However, when it comes to sudden emergencies, are one of the first communication methods to degrade or become completely unusable. Cell towers have a limited amount of bandwidth, and in emergencies, quickly become saturated with requests and will stop being able to help you make calls and texts. Calls are the first thing to stop working. If you attempt to make a call and it fails, attempt to send a text message. Depending on the cell tower's busyness, you may still be able to use that method of communication.
Though somewhat rare, cellular communication can also fail from infrastructure issues due to extreme weather, intentional attacks, or normal electrical/software problems.

I will note that, for several months, it has been known that foreign threat actors have hacked into major U.S. Telecom networks and likely have full access to the same data cellular companies have of your SMS texts and voice calls, which is all of it. Regardless of which third party may attempt to have access to your communication at any given time, if privacy or security is a concern at all for the communication you are doing, you should use end-to-end encryption to ensure only you and the person/people you are talking with can view that content. This is the case for RCS text messages and some other communication protocols or apps I will mention below.


## Internet
Most other communication you are likely familiar with that don't fall into the other categories are considered internet communication. Examples include email, Zoom, Slack, Teams, Facebook, WhatsApp, and most other messaging apps. Internet communication is extremely flexible, and reliability can vary. The availability of cellular data has similar attributes to voice calls, but with even more volatility in the event of high demand. Home networks are less susceptible to slow downs due to demand, but depend on your home having electricity and there not being service outages.

Email is probably the most common, and subsequently, one of the better options for certain communications, however, other communication formats are often more convenient for a lot of back-and-forth or group messaging. Additionally, email is an inherently insecure protocol and should not be used for transmitting any sensitive or private data. If you would like to use email for secure communications, you should use PGP encryption on top of your emails (fairly complicated) or agree with those you communicate with to both use the same email provider who performs end-to-end encryption by default for emails to others with the same domain. The main email providers who do this are Proton Mail and Tuta Mail.

For secure/private internet communication, there are many options. It is generally quite simple to use a single service/app as it only gives users one option for how to communicate. An example would be requiring all communicating parties to download Slack. Another method is deciding on a protocol instead of an app. An example is SMS and RCS text messages or email. Users can choose which app they use (for example, iMessage or Google Messages for texts and Gmail or Proton Mail for email). This adds a little bit of initial complexity for the sole fact that users have to choose between several options of apps, as well as the apps for different platforms (Android, IOS, desktop) being named differently. It does allow more flexibility, however, and doesn't tie you down to a specific app/service. You can pick the interface you enjoy the most.

The below options all allow for text messaging, voice and video calls, and file transfer. They are also cross-platform (you can use them on Android, IOS, Window, Mac, and Linux).
For the single app options, I would recommend [SimpleX Chat](https://simplex.chat) or [Signal Messenger](https://signal.org). For the protocol options, I would recommend [XMPP](https://xmpp.org) or [Matrix](https://matrix.org).


## Radio
Outside of in-person communication, we generally rely on other people's infrastructure (cell towers, servers, etc.). This is fine most of the time, however, being in control of all of the hardware required for distance communication can give you a lot of independence. This is where radio communication shines.

### Walkie-talkies
You are probably familiar with the handheld radios commonly referred to as walkie-talkies. These radios operate on a specially-allocated set of frequencies that, in the radio world, are commonly called FRS (Family Radio Service) frequencies. These radios don't require a license to operate and are legally limited in their function and power output. These radios generally display "channels" instead of the actual frequency they are using (Channel 1 is easier to say than 462.5625 MHz). For reasons we will mention in the ham Radio section, for emergency purposes, you may want a ham radio instead of a walkie-talkie. Most ham radios don't, by default, have the walkie talkie frequencies programmed in to correspond to their channel number. For that reason, I am adding a table that shows the correspondence between the two, so that if you have a ham radio, you can still communicate with someone who only has a walkie-talkie. Please note the legal restrictions with this in the ham radio section.

| Frequency | Channel Number |
| --------- | --------- |
| 462.5625 | Channel 1  |
| 462.5875 | Channel 2  |
| 462.6125 | Channel 3  |
| 462.6375 | Channel 4  |
| 462.6625 | Channel 5  |
| 462.6875 | Channel 6  |
| 462.7125 | Channel 7  |
| 467.5625 | Channel 8  |
| 467.5875 | Channel 9  |
| 467.6125 | Channel 10 |
| 467.6375 | Channel 11 |
| 467.6625 | Channel 12 |
| 467.6875 | Channel 13 |
| 467.7125 | Channel 14 |
| 462.5500 | Channel 15 |
| 462.5750 | Channel 16 |
| 462.6000 | Channel 17 |
| 462.6250 | Channel 18 |
| 462.6500 | Channel 19 |
| 462.6750 | Channel 20 |
| 462.7000 | Channel 21 |
| 462.7250 | Channel 22 |

You may be aware that many walkie-talkies have sub-channels or "privacy-tones". For example, instead of just setting your radio to channel 3, you could set it to 3-1 or 3-8. The 1 and 8 are the extra option that allows you to essentially treat one channel like many different channels, thus allowing more communication within the same frequency range. "Privacy-tones" is an extremely deceptive name. These CTCSS tones (their official name) do not prevent others from hearing your communication. In our example, if you were tuned into channel 3 on your radio, you would be able to hear every other person on channel 3, regardless of the sub-channel/CTCSS tone. The extra setting is just for your own convenience to not have to hear every other person on that channel. 

Again, in ham radios, you also have the option to use these CTCSS tones to gain the same effects of the sub-channels. In order to do this, you would have to enter in the corresponding tone for the T-CTCSS (transmit) and R-CTCSS (receive) settings in your radio. That will tell your radio to both transmit and receive with this special tone, thus blocking unwanted signals from other parties.

| Sub-channel | CTCSS tone |
| ----------- | ---------- |
| 1  |	67.0  |
| 2  |	71.9  |
| 3  |	74.4  |
| 4  |	77.0  |
| 5  |	79.7  |
| 6  |	82.5  |
| 7  |	85.4  |
| 8  |	88.5  |
| 9  |	91.5  |
| 10 | 	94.8  |
| 11 | 	97.4  |
| 12 | 	100.0 |
| 13 | 	103.5 |
| 14 | 	107.2 |
| 15 | 	110.9 |
| 16 | 	114.8 |
| 17 | 	118.8 |
| 18 | 	123.0 |
| 19 | 	127.3 |
| 20 | 	131.8 |
| 21 | 	136.5 |
| 22 | 	141.3 |
| 23 | 	146.2 |
| 24 | 	151.4 |
| 25 | 	156.7 |
| 26 | 	162.2 |
| 27 | 	167.9 |
| 28 | 	173.8 |
| 29 | 	179.9 |
| 30 | 	186.2 |
| 31 | 	192.8 |
| 32 | 	203.5 |
| 33 | 	210.7 |
| 34 | 	218.1 |
| 35 | 	225.7 |
| 36 | 	233.6 |
| 37 | 	241.8 |
| 38 | 	250.3 |

Many walkie-talkies will advertise communication ranges of around 30 miles. In a neighborhood without a clear line of sight, you will be lucky to get one mile. If you have direct line of sight to the person you are communicating with, you may be able to get several miles, but unless you are elevated, the curvature of the earth will quickly limit your range to about 6 miles. For longer-range radio communication, look at the next radio sections.


### LoRa/Meshtastic
A lesser-known radio communication method is using the LoRa (Long-range) modulation technique (you don't need to know what that means). A popular way of doing this is known as Meshtastic. With this communication method, you are able to communicate long distances, encrypt your messages, and share your location, all without needing any radio license. The main downside is the limited bandwidth, which means that you aren't able to communicate with voice messages, only text. These radios do something known as mesh-networking. This means that in a hypothetical situation where three individuals have Meshtastic radios (person 1, 2, and 3), if person 1 wanted to send a message to person 3, but was out of range, as long as person 2 was between them, the message would get to person 2 and person 2's radio would then re-transmit that message, which is hopefully received by person 3. This means that I can communicate with people that are much farther away by hopping the signal through multiple people. Throughout Utah valley, I have frequently connected to people that are 70 miles away.

I have frequently used these radios while camping, backpacking, and hunting to track the location of my family/friends. If you're willing to forgo voice communication (like the radio communication you are likely familiar with), Meshtastic can be an extremely useful and beginner-friendly way to get some good capabilities. The battery life on the radios can frequently be 5-7 days. The lack of a licensing requirement opens the opportunity to many people, but it also constrains the legal power output of the radios. Even though the radios get a surprising range considering the low power output, it is still a low power output, and subsequently, can't perform as well as ham radios that transmit with significantly more power.

If you are slightly tech-savvy and willing to watch a couple of tutorials, you can put one of these radios together (Plug in a battery and clip on a different antenna) for fairly cheap (\$35-\$45).
[Radio](https://store.rakwireless.com/products/wisblock-starter-kit?variant=41786685063366)
[Battery](amazon.com/gp/aw/d/B091Y3TW9F) (You can find these batteries for about $6 when not ordering from Amazon. Also, the positive and negative wires on this need to be swapped in the plastic connector. It isn't too hard to do, but let me know if you are planning on doing this, and I can help.)
A different antenna is not necessary, but recommended for increased range performance. I will try to add more information here on the assembly process, but until that happens, please contact me and I'd be more than happy to help. Putting one of these radios together sounds intimidating, but it is quite simple (I'm probably biased though).

You can also pick from a variety of pre-build solutions. [This is one example](https://store.rakwireless.com/products/wismesh-pocket)

### Ham Radio
Ham radio is extremely diverse. From using a radio as a glorified walkie-talkie to bouncing Morse code radio waves off of the atmosphere to talk to people on the opposite side of the world. There is plenty of room for any experience level, and you can get started without needing to be a major nerd or even having a license. In the United States, the FCC designates certain frequency ranges to be available to amateur (ham) radio operators. To maintain some organization within these limited frequencies, there are licensing and usage laws for transmitting. Receiving (listening), however, is completely legal without any license. For general preparedness, even being able to listen to what others are saying can be extremely useful. There are some recommendations for getting started a few paragraphs below.

Even though you can buy a radio and listen, I still strongly encourage getting a ham radio license. It does require taking a small test, however, there are many study resources and the exam is frequently passed by young children. No preexisting radio knowledge is necessary. Without a license, you will be extremely limited in your motivation to learn more and your ability to practice a potentially life-saving tool. I recommend getting a radio for receiving, even if you never intend on getting a license, however, you wouldn't want your first time driving to be when you have to rush someone to the hospital and your only experience is watching videos tutorials on how to drive. Similarly, don't expect to feel comfortable using ham radio in an emergency if you just don't use it. The tool is still good to have; just don't get complacent in thinking you are prepared. In certain emergencies, an unlicensed user could justifiably transmit on the ham radio frequencies, but you would still need to know what frequency to use and how to operate your radio. See below for what counts as one of these emergencies.

Earlier, it was mentioned that many ham radios are capable of communicating on the frequencies used by walkie-talkies. The FCC, however, has laws around the walkie talkie channels that may make this unlawful, depending on your radio. The primary concerns are that of transmit power and antenna connection. FRS channels have power limits of 2W on all channels except 8-14, which have a limit of 0.5W. Additionally, the antenna is not allowed to be removable on the radio you use on these frequencies (though this is not something that could be known without visual inspection of the radio). For most ham radios, the antenna is removable, and unless it is an emergency, you would technically be using a "non-allowed" radio if you were to talk on the walkie-talkie channels. Violations of FCC rules can result in serious fines. If communicating with walkie-talkies is a primary concern, you should get a walkie-talkie (FRS radio).

#### Example Radios
These are a few, cheap handheld ham radios. They are all fairly popular and it shouldn't be too difficult to find guides and videos for your specific radio (on top of the one that will come with the radio). If you would like a radio that is a little nicer than the ones below, I am going to leave it up to you to find one that will suit your needs, desires, and budget. There are too many radios for me to mention, so this list is primarily targeted at those that aren't super interested in ham radio, don't want to spend very much, but still would like something. None of these radios are flagship devices, but they are fairly common, even among more involved ham radio operators.

- [Baofeng UV-5R](https://www.baofengradio.com/products/catalog-uv-5r)
- - Arguably the most common radio. It is very cheap and has a simple user interface. Because of how common it is, resources are plentiful.
- - [Buy here](https://www.amazon.com/Baofeng-UV-5R-136-174-400-480Mhz-1800mAh/dp/B074XPB313?th=1)
- [Baofeng UV-9R Pro](https://www.baofengradio.com/products/uv-9r-pro?_pos=9&_ss=r)
- - This is basically a UV-5R (the one mentioned above), but waterproof. A little more expensive, but if you need a waterproof radio, this is one of the main budget options.
- - [Buy here](https://www.amazon.com/BAOFENG-Dustproof-Waterproof-Transceiver-Plus%EF%BC%88Green%EF%BC%89/dp/B09J8GWC6D)
- [TidRadio TD H3](https://tidradio.com/products/h3-ham-radio)
- - This radio adds more frequencies compared to the Baofengs (this allows listening to a lot more and being able to talk on frequencies that other people's radios might not be able to, which can help in busy situations). It also allows wirelessly programming the settings of the radio (like labeling a frequency with a specific number or name for easier usage). You can use an app on your phone, which is easier for many people. You can also use a pre-programmed radio to program other radios wirelessly. This is also a great option for usage as a "walkie-talkie". There is another type of radio that wasn't discussed here called GMRS, which for simplicity, we can consider a fancy walkie-talkie. There is a mode for the radio that can convert the radio from a ham radio to a GMRS radio. This allows you to use this without fear of unknowingly breaking any ham radio laws, while giving you the practice of using the radio and the hardware that is capable of it if you were to ever need or want it. Operating a GMRS radio does require a license, but there isn't any test and the license applies to your entire family. See below on how to get this license.
- - [Buy here](https://www.aliexpress.us/item/3256807686983929.html?levelOneExtF=%5Bobject%20Object%5D)
- [Quansheng UV-K5](https://en.qsfj.com/products/3002)
- - For about the same price as the UV-5R, this is arguably a much better radio. The only downside is that it isn't quite as prolific, but it's features have led to it becoming quite popular recently. It has more frequencies it can operate on, which can be extremely useful, especially for listening. Additionally, if you are interested in getting a little more involved, but still want to stick to a budget, this radio has open-source firmware. People have made new features of the software that this radio can run and have given it a ton more capabilities. If you want to tinker, this is a great radio to do so.
- - [Buy here](https://www.aliexpress.us/item/3256807603227075.html?utparam-url=scene%3ApcDetailTopMoreOtherSeller%7Cquery_from%3A)

#### Emergencies
> § 97.403 Safety of life and protection of property.
> 
> No provision of these rules prevents the use by an amateur station of any means of radio communication at its disposal to provide essential communication needs in connection with the immediate safety of human life and immediate protection of property when normal communication systems are not available.

In other words, if you don't have a ham radio license, in a circumstance where there is an essential communication need to save life or property and no other communication methods are available, you may be justified to use the ham frequencies to help solve the problem.

In an emergency, the two main frequencies you would want to use are 146.520 MHz and 446.000 MHz. These are "calling frequencies" and are basically the default frequencies for starting communications (even non-emergency ones). You generally start a conversation on one of these frequencies and then choose to switch to another one if possible. The walkie-talkie channel 20 (462.675 MHz) is the GMRS emergency frequency. 

#### Resources
If you would like to get your ham radio license, I recommend looking at this site
[https://hamstudy.org/](https://hamstudy.org/)

Steve Whitehead, a serious ham operator in Payson, is also a great resource. He frequently helps people get their licenses. I don't want to put his email address on a publicly available site that can be scraped by scammers. If you would like his email, you can either contact me, find it on the Member Tools app, or figure it out from this hint. His ham radio call sign is nv7v. His email username is his call sign and he has a custom domain that is also his call sign with the '.org' tld. An email address is in the format username@domain.tld. So his email is callsign@callsign.org (insert his actual call sign).

Steve also puts on the Payson ham net (meeting over radio) on Sunday evenings at 8:00 PM. To tune in, you can set your radio to the frequency 147.400 MHz (or 447.000 MHz and set your radio setting for tone to +100 Hz). Again, unless you have a ham license, you are only legally allowed to listen.

To get a GMRS license, visit [this site](https://www.fcc.gov/wireless/universal-licensing-system). You first need to register with the FCC, then you can apply for the license.

#### Other Ham Radio References
https://www.radioreference.com/db/browse/ctid/2801
https://www.radioreference.com/db/aid/8851
https://user.xmission.com/~uarc/netsched.html
https://utahvhfs.org/bandplan1.html

