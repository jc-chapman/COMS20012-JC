# Lecture 3 - Cryptography and Web Security

The material is subdivided in small videos.

Please, watch the videos and go through the reading material in your own time.

Also remember to work on the accompanying [exercises sheet](../exercises/EXERCISES3.html)

| Video                   | Links                     |        Reading Material                                                                                                                                                                                      |
|-------------------------|---------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Introduction to Cryptography | [video](https://web.microsoftstream.com/video/1fdf3361-4fbe-4f2b-9f8a-9212ff7ec097?list=studio)  [pdf](https://github.com/cs-uob/COMS20012/blob/master/docs/slides/W3-L1-Intro-Crypto.pdf) | Text Book Chapter 1-- sections 3.1, 3.2, 3.4, 3.5 |
| Introduction to Web Security  | [video](https://web.microsoftstream.com/video/fab39743-9d8d-4727-a09e-389d9349c535?list=studio) [pdf](https://github.com/cs-uob/COMS20012/blob/master/docs/slides/W3-L2-Intro-BasicWebA.pdf) | Text Book Chapter 7-- sections 1.1|
| Web Security Part 1 (XSS, CSRF) | [video](https://web.microsoftstream.com/video/0f9d40b7-89fd-4774-88db-b1ea3ae61e51?list=studio) [pdf](https://github.com/cs-uob/COMS20012/blob/master/docs/slides/W3-L3-Intro-WebSec2-.pdf)| Text Book Chapter 7-- sections 2.6, 2.7|
| Web Security Part 2 (SQLi)  | [video](https://web.microsoftstream.com/video/3e7d3ef8-2ecb-45a2-bba2-ddf7cf4b25b3) [pdf](https://github.com/cs-uob/COMS20012/blob/master/docs/slides/W3-L3-Intro-WebSecA3.pdf) | Text Book Chapter 7-- section 3.3|

## Last week survey results

The results from last week survey are [available](../surveys/week2.html).

## Q&A
**Note:** Due to some setting issues, we realized that when Sanjay was explaining the input Sanitization example, the video did not capture his on-screen writing. It only captured his voice describing the example, which makes it hard to understand what was being pointed out. So, here is the example, he was talking about: It was a real example from MS sanitizing inputs for its IIS server. The idea was to remove the string `<script>` entirely whenever it appears in some specific user input. This will prevent malicious user from inserting javascript. As usual, the mitigation was bypassed by using the following string `<scri<script>pt>`. As you can see, on receiving this string, sanitizer removes substring `<script>`, which results in concating the remaining parts thereby generating the intended string `<script>`.

<iframe width="640" height="360" src="https://web.microsoftstream.com/embed/video/6b66ca13-12ab-4bde-9f97-1150234ae3aa?autoplay=false&amp;showinfo=true&amp;st=4" allowfullscreen style="border:none;"></iframe>
