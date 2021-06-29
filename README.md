Last login: Tue Jun 29 07:32:57 on ttys000
deborahosagie@Deborahs-MacBook-Pro ~ % git
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone     Clone a repository into a new directory
   init      Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.
deborahosagie@Deborahs-MacBook-Pro ~ % git https://github.com/Debby77/Anewme.git 
git: 'https://github.com/Debby77/Anewme.git' is not a git command. See 'git --help'.
deborahosagie@Deborahs-MacBook-Pro ~ % git clone https://github.com/Debby77/Anewme.git
Cloning into 'Anewme'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
deborahosagie@Deborahs-MacBook-Pro ~ % cd Desktop/GitHub
cd: no such file or directory: Desktop/GitHub
deborahosagie@Deborahs-MacBook-Pro ~ % cd Desktop
deborahosagie@Deborahs-MacBook-Pro Desktop % cd Documents
cd: no such file or directory: Documents
deborahosagie@Deborahs-MacBook-Pro Desktop % cd GitHub
cd: no such file or directory: GitHub
deborahosagie@Deborahs-MacBook-Pro Desktop % cd .. 
deborahosagie@Deborahs-MacBook-Pro ~ % cd Documents
deborahosagie@Deborahs-MacBook-Pro Documents % cd GitHub
deborahosagie@Deborahs-MacBook-Pro GitHub % ls
Anewme		Server-code
deborahosagie@Deborahs-MacBook-Pro GitHub % cd Anewme
deborahosagie@Deborahs-MacBook-Pro Anewme % ls
README.md
deborahosagie@Deborahs-MacBook-Pro Anewme % vi README.md                       

for line in handle:
    if line.startswith ('From '):
        words = line.split()
        #print (words)
        stop = words[1]
        #print(stop)
        real.append(stop)
#print (real)

di = dict() 
    
for word in real:
    di[word] = di.get(word,0)+1
#print (di)
  
bigcount = 0
bigword = None
for key,value in di.items():
    if bigcount is 0 or value > bigcount:
        bigcount = value
        bigword = key

print (bigword,bigcount)
-- INSERT --
