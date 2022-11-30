CMPUT404-assignment-websockets
==============================

CMPUT404-assignment-websockets

See requirements.org (plain-text) for a description of the project.

Make a shared state Websockets drawing program

Prereqs
=======
Create a virtual environment and install the required dependencies.

```bash
virtualenv venv --python=python3
source venv/bin/activate
pip install -r requirements.txt
```

Contributors / Licensing
========================

Generally everything is LICENSE'D under the Apache 2 license by Abram Hindle.

freetests.py is LICENSE'D under a BSD-like license:

From ws4py

Copyright (c) 2011-2014, Sylvain Hellegouarch, Abram Hindle
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

 * Redistributions of source code must retain the above copyright notice,
   this list of conditions and the following disclaimer.
 * Redistributions in binary form must reproduce the above copyright
   notice, this list of conditions and the following disclaimer in the
   documentation and/or other materials provided with the distribution.
 * Neither the name of ws4py nor the names of its contributors may be used
   to endorse or promote products derived from this software without
   specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
POSSIBILITY OF SUCH DAMAGE.

Contributors
============

* Landberg: helped me figure out how to set up read_ws to set the current
  state of the world. Also help me figure out what to do with addEntity (just suggestions
  on how to implement it), socket.onOpen (one line of code given, but most based on suggestion)
  and socket.onMessage (help with suggestion and clarify issue i was having).
* rmo1: Explain how sockets.onOpen should work
* og: Helped me fix my socket.onOpen and socket.onMessage so that it is proper (worked before but was
  not properly coded). Also helped me fix socket.py so that the current state would show up if new tab
  was opened (so if something is drawn, it will show up). Helped me fix set_listener and read_ws.

Code
=====

* Most code for sockets.py came from CMPUT 404 lecture 
  * links: https://uofa-cmput404.github.io/cmput404-slides/09-Websockets.html#/25, https://github.com/uofa-cmput404/cmput404-slides/tree/master/examples/WebSocketsExamples
* Some code (mostly for the design of the canvas and circles) came from my assignment 4 code
  * links: https://github.com/happycat33/CMPUT404-assignment-ajax