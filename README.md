Download Link: https://assignmentchef.com/product/solved-comp1400-lab1-unix-exercise
<br>
Both Cygwin (on PC) and Ubuntu (on CS system) are essentially variants of UNIX. While a list of common UNIX commands and control sequences is provided at the end of this file, the following shows a couple of examples for the use of ls command. The base directory is

/cygdrive/c in Cygwin for the C: drive on PC or /home/your user name in Ubuntu, where user name is your user name for login. The following line of command allows you to see the directories and files in the base directory, in which base dir needs to be replaced by either /cygdrive/c or /home/your user name depending on the system you are using.

$ ls base dir

If you have a directory named Program Files in the base directory, the following command lists the files under this directory.

$ ls base dir/”Program Files”

Accomplish the following tasks, and submit your list of commands for the sequence of tasks.

<ol>

 <li>Start a Cygwin terminal (on PC) or Ubuntu terminal (lab machine).</li>

 <li>At the terminal prompt $, create a fall16 directory in the base directory.</li>

 <li>In a similar manner, create a cs140 directory in the newly created fall16</li>

 <li>Change your working directory by going to the /base dir/fall16/cs140</li>

 <li>Check the name of your current working directory.</li>

 <li>List all the files of the current directory, including hidden “dot” files.</li>

 <li>Take one or more (if one is not enough) screenshots, and submit them as your solution to this exercise.</li>

 <li>RAPTOR Exercise:

  <ol>

   <li>Start RAPTOR and create a flowchart to swap two integer numbers entered by the user and display the numbers before and after swapping.</li>

   <li>Run the flowchart with different numbers .</li>

   <li>Save the flowchart to a file named “rap” in the working directory on the PC you are using.</li>

   <li>Demonstrate the rap file to GA/TAs and run with different input values. <em>Hint: For swapping two numbers you need a temporary variable.</em></li>

  </ol></li>

 <li>Basic C Programming Exercise Accomplish the following tasks.

  <ol>

   <li>Start a text editor, which could be gedit on a Ubuntu machine or Notepad++ on PC.</li>

   <li>Type in the program in Section 2.1 on page 10 of the textbook with a modification to change the printf statement to the following, where my name needs to be replaced by your full name.</li>

  </ol></li>

</ol>

printf(“Good morning!∖nMy name is my name.∖n”);

<ol>

 <li>Save the file in the format of a C source file as modified pun.c in your working directory,</li>

</ol>

i.e., /home/your user name/fall16/cs140.

<ol>

 <li>As you are already in the working directory as completing UNIX Exercise, you can now compile the C program with the following command to produce an executable.</li>

</ol>

$ gcc -Wall modified pun.c -o my prog

<ol>

 <li>Run the executable with the following command to produce the output.</li>

</ol>

$ ./my prog

<ol start="4">

 <li>Algorithm implementation with C programming:

  <ol>

   <li>Implement the algorithm as represented by “rap” that you have already created in this lab, and write an equivalent C program that accomplishes what the flowchart does, with the assumption that the input numbers are always integer. You can use scanf to get the values entered by the user. A sample output is shown below:</li>

  </ol></li>

</ol>

Enter the first number: 5

Enter the second number: 10

Before swapping, the first number was 5 and the second number was 10.

After swapping, the first number is 10 and the second number is 5.

<ol>

 <li>Save your program to a file named “c”, in the working directory on the PC you are using.</li>

 <li>Demonstrate the c file to GA/TAs and run with different input values.</li>

</ol>

<em>NOTE: Files saved on the PCs in the lab are not be permanent. They must be either saved to a USB drive, or transferred to Ubuntu.</em>

<strong>COMMON COMMAND AND CONTROL SEQUENCES </strong>The following commands can be entered at the UNIX system command prompt. Press the ⟨Return⟩ key after each command. Use lower case letters unless otherwise indicated.

<table width="0">

 <tbody>

  <tr>

   <td width="175">Command</td>

   <td width="501">Description</td>

  </tr>

  <tr>

   <td colspan="2" width="676">WORKING WITH DIRECTORIES</td>

  </tr>

  <tr>

   <td colspan="2" width="676">pwd                                    Gives you the name of your current working directory.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">cd dirname Changes your working directory to dirname. If you are not in dirname’s parent directory, you must use dirname’s full pathname.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">cd .. Changes your working directory to the parent of the directory that you are in when you issue this command. If you are at the root, you will remain there.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">cd                                       Changes your working directory to your home directory.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">ls                                         Lists the files in your working directory.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">ls -l Lists the files in your working directory, giving lengthier information about them — including file protection and access privileges.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">ls -a Lists the files in your working directory and shows your hidden “dot” files, as well, including your .login file.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">ls -lt                                       Same as ls -l, but orders the files by time modified.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">mkdir dirname                      Creates a directory called dirname.Your working directory will be the parent of this new directory, unless you specify another pathname.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">rmdir dirname Deletes a directory called dirname, if the directory is completely empty. If you are not in dirname’s parent directory, you must use dirname’s full pathname.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">WORKING WITH FILES</td>

  </tr>

  <tr>

   <td colspan="2" width="676">pico filename Uses the editor pico to open a file called filename. If a file of that name does not already exist, it starts a new one.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">vi filename                             Uses the editor vi to open a file called filename.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">cp file1 file2 Makes a copy of a file called file1 and names the copy file2. If there already is a file called file2, it will be replaced.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">cp -i file1 file2                    Makes a copy of file1 and calls the copy file2. If there already is a file called file2, the system queries you before replacing it.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">rm filename                           Deletes a file called filename.If you are not in the same directory as filename, you must specify filename’s pathname.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">rm -i filename                       Deletes a file after confirmation. Type y to confirm, n to cancel.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">more filename Lists the contents of the file called filename on your screen. Press the spacebar to scroll forward in the file. Type b to scroll back one screenful.Type q to quit.</td>

  </tr>

  <tr>

   <td colspan="2" width="676">lpr -P pr fname                      Sends a file called fname to a printer called pr.</td>

  </tr>

 </tbody>

</table>

<table width="0">

 <tbody>

  <tr>

   <td width="676">ADDITIONAL COMMANDS</td>

  </tr>

  <tr>

   <td width="676">history                                 Lists your previous commands. !n Executes command number n in the list that you receive as output of the history command.</td>

  </tr>

  <tr>

   <td width="676">man command Obtains online information about the command of your choice. These are the UNIX system’s online “man pages”.Press the spacebar to scroll to the next screenful. Type b to scroll back a screenful. Type q to quit the man facility.</td>

  </tr>

  <tr>

   <td width="676">man -k key Obtains online information when you do not know the command name. Replace key with a keyword for the function you wish to perform.</td>

  </tr>

  <tr>

   <td width="676">learn                                      Initiates online instruction in file manipulation, vi, C, and other topics.</td>

  </tr>

  <tr>

   <td width="676">passwd Initiates the password-changing program. Respond, as prompted, with your old and new passwords.</td>

  </tr>

  <tr>

   <td width="676">pine                                      Starts the Pine mail program.</td>

  </tr>

  <tr>

   <td width="676">tin                                        Starts the network news reader tin. Use the up- and down-arrow keysto highlight a newsgroup (or message) of interest; press Enter key to select it. Type ? for help, and q to quit.</td>

  </tr>

  <tr>

   <td width="676">logout                                  Logs you off the UNIX system.If you have a “stopped process”, the system will prompt you. Enter fg to resume the process or logout a second time to abort the process and log off the system.</td>

  </tr>

  <tr>

   <td width="676">KEYS AND TERMINAL EMULATIONIn the following, a caret (<sup>∧</sup>) indicates the “control” key (often marked CTRL or CTL). Hold the “control” key down while typing the letter shown next to it.</td>

  </tr>

  <tr>

   <td width="676">Backspace To backspace, use the backspace key (often marked BKSP) or, if that does not work, the delete key (often marked DEL).</td>

  </tr>

  <tr>

   <td width="676"><sup>∧</sup>c                                        Aborts the current process — e.g., a long screen listing.</td>

  </tr>

  <tr>

   <td width="676"><sup>∧</sup>s                                        Temporarily suspends a listing until you type <sup>∧</sup>q.</td>

  </tr>

  <tr>

   <td width="676"><sup>∧</sup>q                                        Resumes a listing after it has been suspended with <sup>∧</sup>s.</td>

  </tr>

  <tr>

   <td width="676">MORE CONTROL KEY SEQUENCES (ADVANCED USAGE)</td>

  </tr>

  <tr>

   <td width="676">u Erases the whole line of characters you have typed thus far at the command line.</td>

  </tr>

  <tr>

   <td width="676"><sup>∧</sup>d                                        This is the end-of-file indication.</td>

  </tr>

  <tr>

   <td width="676">z Suspends the execution of a process/”job”. You may then have the process continue in the background (type bg immediately after). Type fg to resume the job or bring it to the foreground. To kill a suspended job, type jobs, then kill %n, where n is the number of the suspended job. (Note: use of this suspend character should be avoided until you have some familiarity with the system.)</td>

  </tr>

 </tbody>

</table>