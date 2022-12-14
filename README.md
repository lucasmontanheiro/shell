# shell

## Basic

<img src="img/layers.jpg">

### 01 Hello World
To edit a file in shell, hit

```
nano helloworld.sh
```

To save and get out of nano, hit `CTR + X` and then hit `Y`.
To run: `bash helloworld.sh` or `.\helloworld.sh`
But first you need to give permission: `chmod +x helloworld.sh`

**Basic commands for this lesson:**
```
echo 		#to print a message or variable
chmod 		#to change permissions in files or directories
exit 		#to exit terminal or connection
```



### 02 Variables

```
read $name  #for user input

name="assign text to a variable"

echo "It will use your variable here: $name"
```

To use an input directly from shell, like `.\BestDay.sh eggs`, use `$1` for the first parameter
```
recipe=$1
echo "Today I'm going to cook $recipe"
```

**Basic commands for this lesson:**
```
whoami 		#your username
date 		#current date and time
pwd			#where in directory you are
```



### 03 Basic Math
```
echo $SHELL 		#your shell
echo $USER 			#your userid
echo $HOSTNAME		#your hostname
```

To create a new variable name for your system:
```
$ bestteam="Corinthians"
$ echo $bestteam
```
That can be used in your script!

But that will be erased as soon as you restart your terminal. To make it permanent, you need to write into a file called `.bashrc`. The `.` means that the file is hidden. That's a script that will run every time the system logs in. 

```
nano .bashrc
```

Add `export bestteam="Corinthians"` at the end of the file and log out and log in. 

```
echo $bestteam		#will equals to Corinthians!
```





## Cool commands

**Basic commands**
```
tree 	// shows the whole directory
mkdir 	// create a directory
```

**Network commands**
```
ipconfig
ipconfig /all
findstr
ipconfig /release
ipconfig /renew
ipconfig /displaydns
ipconfig /renew
clip
ipconfig /flushdns
nslookup
cls
getmac /v
```

**Check Battery**
```
powercfg /energy
powercfg /batteryreport
assoc
```

**Is your computer slow?**
```
chkdsk /f
chkdsk /r
sfc /scannnow
DISM /Online /Cleanup /CheckHealth
DISM /Online /Cleanup /ScanHealth
DISM /Online /Cleanup /RestoreHealth
tasklist
taskkill
netsh wlan show wlanreport
netsh interface show interface
netsh interface ip show address | findstr ???IP Address???
netsh interface ip show dnsservers
netsh advfirewall set allprofiles state off
netsh advfirewall set allprofiles state on
ping
ping -t
tracert
tracert -d
netstat
netstat -af
netstat -o
netstat -e -t 5
route print
route add
route delete
shutdown /r /fw /f /t 0
```


## Changing files permissions

```
chmod ugo+rwx foldername
```



## Resources

- [ ] [Article: Streamline your projects using Makefile](https://dev.to/yankee/streamline-projects-using-makefile-28fe)
- [ ] [Article: Understand Linux Load Averages and Monitor Performance of Linux](https://www.tecmint.com/understand-linux-load-averages-and-monitor-performance/)
- [ ] [Article: Command-line Tools can be 235x Faster than your Hadoop Cluster](https://adamdrake.com/command-line-tools-can-be-235x-faster-than-your-hadoop-cluster.html)
- [ ] [Calmcode: makefiles](https://calmcode.io/makefiles/the-problem.html)
- [ ] [Calmcode: entr](https://calmcode.io/entr/introduction.html)
- [ ] [Codecademy: Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line)
- [ ] [Datacamp: Introduction to Shell for Data Science](https://www.datacamp.com/courses/introduction-to-shell-for-data-science)
- [ ] [Datacamp: Introduction to Bash Scripting](https://www.datacamp.com/courses/introduction-to-bash-scripting)
- [ ] [Datacamp: Data Processing in Shell](https://www.datacamp.com/courses/data-processing-in-shell)
- [ ] [MIT: The Missing Semester of CS Education](https://www.youtube.com/playlist?list=PLyzOVJj3bHQuloKGG59rS43e29ro7I57J)
	- [ ] [Lecture 1: Course Overview + The Shell (2020)](https://www.youtube.com/watch?v=Z56Jmr9Z34Q) `0:48:16`
	- [ ] [Lecture 2: Shell Tools and Scripting (2020)](https://www.youtube.com/watch?v=kgII-YWo3Zw) `0:48:55`
	- [ ] [Lecture 3: Editors (vim) (2020)](https://www.youtube.com/watch?v=a6Q8Na575qc) `0:48:26`
	- [ ] [Lecture 4: Data Wrangling (2020)](https://www.youtube.com/watch?v=sz_dsktIjt4) `0:50:03`
	- [ ] [Lecture 5: Command-line Environment (2020)](https://www.youtube.com/watch?v=e8BO_dYxk5c) `0:56:06`
	- [ ] [Lecture 6: Version Control (git) (2020)](https://www.youtube.com/watch?v=2sjqTHE0zok) `1:24:59`
	- [ ] [Lecture 7: Debugging and Profiling (2020)](https://www.youtube.com/watch?v=l812pUnKxME) `0:54:13`
	- [ ] [Lecture 8: Metaprogramming (2020)](https://www.youtube.com/watch?v=_Ms1Z4xfqv4) `0:49:52`
	- [ ] [Lecture 9: Security and Cryptography (2020)](https://www.youtube.com/watch?v=tjwobAmnKTo) `1:00:59`
	- [ ] [Lecture 10: Potpourri (2020)](https://www.youtube.com/watch?v=JZDt-PRq0uo) `0:57:54`
	- [ ] [Lecture 11: Q&A (2020)](https://www.youtube.com/watch?v=Wz50FvGG6xU) `0:53:52`
- [ ] [Thoughtbot: Mastering the Shell](https://thoughtbot.com/upcase/mastering-the-shell)
- [ ] [Thoughtbot: tmux](https://thoughtbot.com/upcase/tmux)
- [ ] [Udacity: Linux Command Line Basics](https://www.udacity.com/course/linux-command-line-basics--ud595)
- [ ] [Udacity: Shell Workshop](https://www.udacity.com/course/shell-workshop--ud206)
- [ ] [Udacity: Configuring Linux Web Servers](https://www.udacity.com/course/configuring-linux-web-servers--ud299)
- [ ] [Web Bos:  Command Line Power User](https://www.youtube.com/watch?v=DP218aBHm1Q&list=PLu8EoSxDXHP7tXPJp5ZmUpuT7sFvrswzf&index=2)
- [ ] [Youtube: GNU Parallel](https://www.youtube.com/playlist?list=PL284C9FF2488BC6D1)
- [X] [YouTube: you need to learn BASH Scripting RIGHT NOW!! // EP 1](https://www.youtube.com/watch?v=SPwyp2NG-bE)
- [X] [YouTube: BASH scripting will change your life](https://www.youtube.com/watch?v=7qd5sqazD7k)
- [X] [YouTube: this BASH script will make you a MILLIONAIRE](https://www.youtube.com/watch?v=19nN9vgcgmU)