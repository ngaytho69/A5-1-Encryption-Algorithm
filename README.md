# A5-1-Encryption-Algorithm
Implementation of A5/1 Encryption Algorithm which is part of our Informations and Security Homework.

* <a href="#Task">Task</a> </br>
* <a href="#Description">Description</a> </br>
* <a href="#Implementation">Implementation</a> </br>

<a id= "Task" ></a>
## Task
This is the task given: 
```C
Implement the A5/1 algorithm. Suppose that, after a particular step, the values in the registers are
X = (x0, x1, . . . , x18) = (1010101010101010101)
Y = (y0, y1, . . . , y21) = (1100110011001100110011) 
Z = (z0, z1, . . . , z22) = (11100001111000011110000)

Generate and print the next 8 keystream bits. Print the contents of X, Y and Z after the 8 keystream bits have been generated. 
```

<a id= "Description" ></a>
## Description
A5/1 is a stream cipher used to provide over-the-air communication privacy in the GSM cellular telephone standard. It is one of seven algorithms which were specified for GSM use.[1] It was initially kept secret, but became public knowledge through leaks and reverse engineering. A number of serious weaknesses in the cipher have been identified.

A5/1 is based around a combination of three linear feedback shift registers (LFSRs) with irregular clocking. The three shift registers are specified as follows:
<table>
  <tr>
    <td>LFSR no.</td>
    <td>Length in bits</td>
    <td>Feedback polynomial</td>
    <td>Clocking bit</td>
    <td>Tapped bits</td>
  </tr>
  <tr>
    <td>1</td>
    <td>19</td>
    <td>x<sup>19</sup> + x<sup>18</sup> + x<sup>17</sup> + x<sup>14</sup> + 1</td>
    <td>8</td>
    <td>13, 16, 17, 18</td>
  </tr>
  <tr>
    <td>2</td>
    <td>22</td>
    <td>x<sup>22</sup> + <sup>21</sup> + 1</td>
    <td>10</td>
    <td>20, 21</td>
  </tr>
  <tr>
    <td>3</td>
    <td>23</td>
    <td>x<sup>23</sup> + x<sup>22</sup> + x<sup>21</sup> + x<sup>8</sup> + 1</td>
    <td>10</td>
    <td>10	7, 20, 21, 22</td>
  </tr>
</table>

![A5/1](https://upload.wikimedia.org/wikipedia/commons/5/5e/A5-1_GSM_cipher.svg)

<a id= "Implementation" ></a>
## Implementation
This is what the output of the program when it is being run on the command line: 

![exe](https://cloud.githubusercontent.com/assets/15609506/26024733/80bec58e-380a-11e7-8ec0-1b77b408a351.png)

