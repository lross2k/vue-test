<template>
  <div class="blog">
    <div class="blog-entry">
      <h1> I wanted to make a blog since long time ago</h1>
      <p>What tech stack	should I use? I'm tired	of using React,	Jekyll doesn't seem that cool 
      to me, vanilla JS is nice but I don't have that much free time, what about Svelte or Vue?</p>
      <p>Well, Svelte sounds cool, but in the terrible case that	I needed job as	frontend 
      developer, I think Vue gives me more validity</p>
      <h2>Installing Vue</h2>
      <p>I needed to install node, for that apparently it's recommended to use nvm, which actually 
      did install node really fast on my system</p>
      <p>The vue installer asked many questions, I said yes to a lot of them, which maybe will 
      leave my computer with no disk space remaining,	but there was only one way to find out</p>
      <p>It installed really fast actually, I'm impressed, now it's time to quickly learn how to 
      do a half decent Vue landing page </p>
    </div>

    <div class="blog-entry">
      <h1> Learning NES 6502 assembly </h1>
      <p>For many years I've wanted to learn assembly, and have read many books and watched
      tutorials on the matter, even assembled basic example programs in different platforms,
      however, I never wrote my own code</p>
      <p>If there is something to blame for my failure, I say it is the huge size of the x86 ISA, I
      understand it's a CISC architecture and all that, but seriously, I feel like I never know
      "enough" to write a simple program, so my solution was to learn assembly in 8 bits, instead of
      32/64 bits, like the good old programmers like Richard Stallman, Dennis Ritchie and Ken
      Thompson had to do in their youth</p>
      <h2>First encounter</h2>
      <p>Initially I set up my environment in Fedora 38, installed CC65 building it from source and
      then installed the Fceux emulator, using RPM Fusion and many other things until I had it
      working, succesfully compiled and debugged a basic ld, st, inc, dec example from youtuber
      NesHacker, this was a quick introduction after reading on the matter and didn't take more than
      3 hours of my saturday morning.</p>
      <h2>Second encounter</h2>
      <p>Same approach but this time I was in another computer, a Debian 12/Unstable desktop
      computer, installed CC65 and Fceux with APT, then jumped straight onto writting this entries
      and then it was time to code more assembly</p>
      <p>I began watching the rest of videos from the quick series of NesHacker, however, it didn't 
      get that far into the NES programming as I expected, so instead I turned into the approach of
      reading an ebook, and I found the "Nintendo Entertainment System Documentation" v1.0 by
      Patrick Diskin, this had all the info I needed, just no hand holding, so it was time to
      practice by hand</p>
      <p>After making some basic code, I wanted to create a TicTacToe "game", but for some reason 
      ended up trying to get random numbers, so I started a mission of writting a random number 
      generator in assembly</p>
      <p>After trying quite a lot, I couldn't make a good random generator, but I also believe 
      generating one will be easier with more changing registers, say with more moving parts 
      in the game it will be easier to get changing values, so I ended up with 2 returning values
      by iterating the ROM data, now I will take a break, but my next challenge will be using the 
      I/O</p>
      <h2>Third encounter</h2>
      <p>Time for I/O, controller is read at $4016, second one at $4017, each of the bits is
      interpreted as A, B, Select, Start, Up, Down, Left, Right respectively.</p>
      <p>I tried reading the inputs and changing memory as a response, but the results were, very
      bad to say the least, so I have a new objective, I'll assume my understanding of basic
      opcodes is enought, as well as my understanding of controller inputs, so I'll jump into
      learning iNES or NES 2.0 formats for showing graphics on the screen, however this also
      requires to create .chr files to load sprite and background characters, which also requires me
      to make sprites in the correct format...</p>
      <p>To learn without going crazy or giving up, I searched resources online, and found a guide
      for exactly most of whay I need, however the video shows a program called YY-CHR but this is
      Windows only, so I'm now searching for a solution, probably will end up using Bottles</p>
      <h2>Resources</h2>
      <ul>
          <li>https://youtube.com/playlist?list=PLgvDB6LWam2WvoFvh8tlUqbqw92qWM0aP</li>
          <li>https://www.nesdev.org/NESDoc.pdf</li>
          <li>http://www.6502.org/tutorials/6502opcodes.html#ADC</li>
          <li>https://dwheeler.com/6502/oneelkruns/asm1step.html</li>
          <li>https://github.com/InkboxSoftware/NESGuide</li>
      </ul>
    </div>
  </div>
</template>

