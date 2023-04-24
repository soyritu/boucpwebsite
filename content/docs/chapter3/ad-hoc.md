---
title: এড-হক প্রবলেম
linktitle: এড-হক প্রবলেম- Ad-hoc Problem
type: book
weight: 10
---
 যেসব প্রবলেমকে অন্য কোনো ক্যাটাগরিতে
 ফেলা যায় না সেগুলাই এড-হক প্রবলেম। আইসিপিসিতে ১০ টা প্রবলেমের মধ্যে কমপক্ষে  ২-১ টা
 এড হক প্রবলেম
থাকে। এড হক প্রবলেম প্রায়গুলাই গেম রিলেটেড যেমন - দাবা,
তাস, ইত্যাদি এবং স্ট্রিং রিলেটেড যেমন প্যালিনড্রম,এনাগ্রাম আবার কিছু 
কনস্ট্রাকটিভ টাইপের হয়ে থাকে।
## যেভাবে এড হক প্রবলেম সল্ভ করতে হয়
এডহক প্রবলেম সমাধান করার কোনো ধরাবাধা নিয়ম নাই।
একেক প্রবলেম একেক ভাবে সল্ভ করতে হয়।
তবে কিছু নিয়ম অনুসরন করলে এডহক দ্রুত সল্ভ করা যাই ।
### ১। প্রয়োজনীয় কথাগুলা নোট করা
একটা প্রবলেমে বর্ণনাতে প্রয়োজনীয় অপ্রয়োজনীয় সব ধরনের কথাবার্তা  থাকে।
শুরুতে এক ঝলক প্রবলেমের বর্ণনা পড়ে প্রয়োজনীয় অংশটুকুই শুধু মার্ক করলে
প্রবলেমটা বোঝা সহজ। 
### ২। আইডিয়াগুলা লিখে রাখা
প্রবলেম পড়ার সময় সল্ভ করার যেসব আইডিয়া মাথায় আসে 
সেগুলো নোট করলে  পরে ভুলে যাওয়ার  সম্ভাবনা থাকে না।
### ৩। একটা আইডিয়াতে নিজেকে লক করে না ফেলা
একটা আইডিয়া মাথায় আসলো শুধু সেটা নিয়ে পড়ে থাকলে হবে না।
যদি শিউর থাকা যায়  এই ওয়েতে সল্ভ হবে সেটা অন্য ব্যাপার।
সব সময় ক্লিয়ার ধারনাটাকে সামনে রেখে আগাতে হবে। কোনো আইডিয়া ক্লিয়ার না হলে সেদিকে না
আগানোই বেটার।
### ৪। ছোট ছোট টেস্ট কেস সল্ভ করা
প্রবলেমে ছোট টেস্ট গুলা সল্ভ করা ট্রাই করা উচিত। প্রবলেমে ঠিক কি চাচ্ছে, কতগুলো  কন্ডিশান হতে পারে, প্রত্যেক টির 
জন্য আলাদা টেস্ট কেস স্টাডি করলে পুরা প্রবলেম টা সলভ করা ইজি হয়ে যাই ।
### ৫। প্রবলেমের প্যাটার্ন ধরা
সব থেকে গুরুত্বপূর্ণ  ব্যাপার হচ্ছে প্রবলেমে কি কি জিনিস ইনিশিয়ালই বা প্রাথমিকভাবে আছে। আর প্রবলেমে যেসব স্টেপ ফলো করতে বলছে ঐগুলা ফলো করলে
পরবর্তীতে কোন অবস্থাতে যাই সেটা বের করা। কয়েকটা কেস স্টাডি করে প্রবলেমের প্যাটার্ন টা ধরতে পারলে এর অ্যালগরিদম ডিজাইন করা সহজ। 
### উদাহরণ- 10490 Die Game UVa
 https://onlinejudge.org/index.php?option=com_onlinejudge&Itemid=8&page=show_problem&problem=1350

Life is not easy. Sometimes it is beyond your
 control. Now, as contestants
of ACM ICPC, you might be just tasting
 the bitter of life. But don’t worry!
Do not look only on the dark side of life,
 but look also on the bright side.
Life may be an enjoyable game of chance, 
like throwing dice. Do or die!
Then, at last, you might be able to 
find the route to victory.

This problem comes from a game using a die. 
By the way, do you know
a die? It has nothing to do with ”death.”
A die is a cubic object with six
faces, each of which represents a 
different number from one to six and is
marked with the corresponding number of spots.
Since it is usually used
in pair, ”a die” is a rarely used word.
 You might have heard a famous phrase 
”the die is cast,” though.
When a game starts, a die stands 
still on a flat table. During the game, 
the die is tumbled in all
directions by the dealer. You will win the game if you can predict the number seen on the top face at
the time when the die stops tumbling.

Now you are requested to write a program 
that simulates the rolling of a die. 
For simplicity, we
assume that the die neither slips nor 
jumps but just rolls on the table in 
four directions, that is, north,
east, south, and west. 
**At the beginning of every game, 
the dealer puts the die at the center
 of the
table** and adjusts its direction so
 that the numbers **one, two, and three
 are seen on the top, north, and
west faces, respectively.**
 For the other three faces, we do
 not explicitly specify anything
 but tell you
the golden rule:
 **the sum of the numbers on any pair
 of opposite faces is always seven.**

Your program should accept a sequence
 of commands, each of which is either
 “north”, “east”,
“south”, or “west”. A “north” command
 tumbles the die down to north,
 that is, the **top face becomes
the new north, the north becomes
 the new bottom, and so on.**
 More precisely, the die is rotated
 around
its north bottom edge to the north
 direction and the rotation angle
 is 90 degrees. Other commands also
tumble the die accordingly to their
 own directions. Your program should
 calculate the number finally
shown on the top after performing 
the commands in the sequence.
 Note that the table is sufficiently
large and the die never falls off 
during the game.
### Input
 
The input consists of one or more 
command sequences,
 each of which corresponds
 to a single game. The
first line of a command sequence
 contains a positive integer,
 representing the number of the following
command lines in the sequence. 
You may assume that this number is less
 than or equal to 1024.
 A line
containing a zero indicates the end
 of the input. Each command line
 includes a command that is one
of ‘north’, ‘east’, ‘south’, and ‘west’.
 You may assume that
 no white space occurs in any lines.
### Output
For each command sequence, output one line containing solely the number on the top face at the time
when the game is finished.
### Sample Input
1\
north\
3\
north\
east\
south\
0
### Sample Output
5\
1


এই প্রবলেমটা একঝলক পড়ার পর আমি প্রয়োজনীয় কথাগুলো বোল্ট করছি।
শুরুতে টপে থাকছে ১ , উত্তরে থাকছে ২ এবং পশ্চিমে ৩। গোল্ডেন রুল অনুযায়ী 
বাকি ৩ টাতে থাকছে (৭ - এর পেয়ার)। যেমন উত্তরের পেয়ার দক্ষিণ এর ভ্যালু ৭-২=৫।
ডাই টাকে যেদিক গড়াবো সেদিকের পেয়ার হবে নিউ টপ আর পুরাতন টপ হবে সেই নতুন সেই দিক।
ব্যাস প্রবলেমের বিষয়বস্তু এতটুকুই । এখন দেখা যাক কতগুলো
কেস আছে। এখানে কেস হবে মোট চারটা কারন ডাই টা উত্তর, দক্ষিণ, পূর্ব ও পশ্চিম এই
চারটা দিকেই শুধু গড়াতে পারবে।
এই কন্ডিশানগুলা এপ্লাই করলেই প্রবলেম সলভ হবে।

## পাইথন সল্ভ
```python3
#infinite loop while input is not 0.
while True:
	t=int(input())
	if t==0:
		break
	else:
		#initial the die:
		top = 1
		down = 7-1 #as golden ratio
		north = 2
		south = 7-2
		west = 3
		east = 7-3
		while t>0:
			t-=1
			d=input()
			old_top=top
			old_down=down
			#small case 1: if input is north
			if d=="north":
				top=south
				down=north
				north=old_top
				south=old_down
			#small case 2: if input is south
			elif d=="south":
				top=north
				down=south
				south=old_top
				north=old_down
			#small case 3: if input is east
			elif d=="east":
				top=west
				down=east
				east=old_top
				west=old_down
			#small case 4: if input is west
			elif d=="west":
				top=east
				down=west
				west=old_top
				east=old_down
		print(top)
```
নিচে কিছু এডহক প্রবলেমের লিংক দিচ্ছি। আশা করা যায় উপরের নির্দেশ অনুসরণ 
করলে সহজ,কঠিন সবগুলা প্রবলেমই কয়েক মিনিটে সল্ভ করা সম্ভব।
