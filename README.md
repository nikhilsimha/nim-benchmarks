# nim-benchmarks
Benchmarks comparing Nim and other languages based on [Programming-Language-Benchmarks](https://programming-language-benchmarks.vercel.app/) by [hanabi1224](https://github.com/hanabi1224/Programming-Language-Benchmarks).

I believe there are quite a few opportunities to improve the benchmarks for nim. My M3 mac currently cannot properly run the benchmarks in the original repo. I aim to eventually merge these changes back into the original repo.  

## Do these benchmarks matter for real-world scenarios?

Some do and others don't  - json parsing / arbitrary precision arithmetic / http serving etc are some things that appear often in real-world scenarios. 

Conventional wisdom is that one picks the right-language-for-the-job™. But most people pick the "right language" based on a combination of taste and circumstance and stick with it. 
No one wants to learn 10 languages to do 10 different kinds of things. I believe nim is flexible enough to solve a very large set of problems without sacrificing dev or machine efficiency.

The nim community, perhaps correctly, doesn't prioritize benchmarks. However, for a language that advertises efficiency as much as nim does, people would want to see numbers before they invest in the language.
My primary goal is to give people looking into to adopting nim more confidence in terms of efficiency.



## How to run?

We compare by using the command like so: `nim c -d:danger --mm:orc pidigits.nim && /usr/bin/time -l ./pidigits 1000`

These print out time and memory consumption along with some other information.






