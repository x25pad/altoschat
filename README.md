**One upon a time ...**

> ... i got some spare time, and a system connected to the X.25 network.
> Soon it became more and more interesting, to start some sort of
> communication with all the hackers coming into that system. The
> system-utilities did not offer too much comfort ( did you ever try to
> talk to three people at the same time using the 'write'-command ? ).
> So i started thinking and playing a little bit and i was investigating
> the features that Xenix 2.5 was offering me for some sort of
> interprocess communication. The results were lousy. Microsoft didn't
> implement the multiplexed files anymore, not to talk of message
> queues, shared memory etc. I could use data-files, of course. Opening
> files exclusively, writing one line of text, closing them again.
> Needless to say another word to that. ... but time went on, new
> operating systems were invented, Microsoft proudly presented their
> first revision of Xenix 3.0, and I got named pipes. What a progress!
> During those days, the second version of my conference-utility started
> its work. A few positive aspects of the named pipes made me keep to
> them: they offer some sort of buffering between the processes, they
> are available on many unix-derivates, they are easy to handle. Many
> features have been included in the meantime, some rework has been done
> on several parts of the software, and some good ideas are still
> pending. As many of the users asked me for that program ( to develop
> it further on ), I thought, it would be a good idea, to put it on the
> network. It's basic concept was to keep it simple and stable. I did
> not include fullscreen-options ( many of the users on the system
> mentioned above just use 300 baud lines ), and I didn't include
> message editing and message lockout ( I'd need all the characters one
> by one, as soon as they are typed in; All the X.25 users would have to
> pay for every character, they are typing ). I hope, you'll enjoy that
> program ( its easy to install ), and let me know, wheather it's
> useful, needs to be improved, or you have any other comments. The
> program is by no means perfect, I know several caveats, minor bugs
> etc. The program has grown from several dozen lines during the years,
> and I still plan to extend it. Feel free to call the system mentioned
> above and have a look to it. (X.25:  0262 45 8900 40004, login:
> guest). My uucp-mail-adress is:   ...!mcvax!unido!altger!korn Hans
> Korneder, DataVision, May 1987

## revision history:

 - 1.0  -  altos 586 xenix 2.5
 - 2.0  -  altos 3068 unixV.2
 - 3.0  -  altos 3068 unixV.2
			 - ascii transfer only
			 - rearranged the location of the named pipes
			 - put to public domain
 - 3.1  -  altos 3068 unixV.2  29.may 1987
			 - rearranged the signal-handling
			 - corrected a problem with sccanf(buf,"%6d",...), that
			 - caused messages starting with numers to be ignored.
			 - ignore empty lines do timeouts for 
				 - a) the server writing to user-answer-pipes
				 - b) opens to user-answer-pipes ( both caused severe problems! )
