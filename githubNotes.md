# +++++++++++++++++++++++++ github notes ++++++++++++++++++++++++++

1) show hidden file command
ls -la

2) check which types of changes you did in your code
git diff

3) github pr koi file & folder push nhi krna chate ho toh command
git rm (file & folder name)

4) check commit history with the help of command
git log

5) check commit history with the short details information
git log --oneline

6) yeh command yeh btangii ki iss commit k ander kya kya changes hue hai (and visualize karna ki iss commit pr kya kya changes huye hai)
git show 232e5c8

7) yeh check karna kiss author ne kiss time pr kon sa code change kiya and kya changes kiya 
git blame index.js

8) check status of file and folder & code
git status

# What is reverting back in github
means apka changes se code fatt gya and yaa kuch issues ho gya then hum reverting back use krte hai humare pass 1 mechanism hota hai ki agr humse kuch guilt ho jata hai toh mein history mein back ja skta hui ise reverting back kehta hai
9) reverting back krne k liye 1 commit upper k changes ko detect karna

git log --oneline

9) reverting back krne k liye 1 commit upper k changes ko detect karna
git reset --hard bdc821d

10) humare pass github pr yeh option bhi hota hai ki hum apne saare commit ko rkhe pr hume upper ke commit mein se code ko remove krna hai usi commit mein yaa fir code ko changes krna hai baad mein per humne kaafi commit kr diye hai aur hume yaad aaya baad mein yaad aaya ki ab woh code change krna hai toh iss case mein hum yeh use kranga 

# Reverting back (why was used reverting back in github) 

git revert <commit-id> kya karta hai?

✔ Old commit ko delete nahi karta
✔ Us commit ka reverse commit bana deta hai
✔ Safe method hai (history safe rehti hai)

# 2 way to do git Reverting back in our code
    - git status
    - git commit -m "Saving current work before revert"
    - git revert fe71839
    - git status
    - git add .
    - git commit -m "Revert something"
    - git log
    - git log --oneline
    - git show

# part - 2 start here

# how can i collaboration with team
vcs => version controling system (full form)
    - git status
    - git diff
    - git add .
    - git commit -m "replace concat with template literals"
    - git push
    - git log --oneline

# agr hum latest command se neecha aana chate hai yaa fr durse commit pr jaana chate hai toh hume yeh command run krni pdangii (how can i remove head in commit)
git reset --hard 0136184

# now you need to push your code
git push -f 

# Branching in Git (learn Branch)

# company/senior require john Doe code to revert (this happen in with the help of branch) (company requirement karti hai ki jo john Doe ka code hai woh buth kharab code hai toh uss code ko revert kro)
    - yha pr hume prblem hongi agr john Doe ke code ko changes ko revert karna chayanga toh kahi naa kahi mra change bhi revert honga agar mein apna head ko reset karna ka try krunga toh kahi naa kahi woh mre changes ko revert kar denga agr mein revert command k use krunga toh agr 3 commit hai toh reality mein 3 commit hai toh woh 3 ko revert krna not possible jab bhi hum collaboration mein work krte hai toh har developer independently apna apna branch bna kr code push krta hai this is best approach in a team.

# short command to check commit and commit time
git log --oneline

# how can i check which type of branch i m there
git branch 

# how can i create new branch
git branch "neha-feature"

# check how much branches you have in your repo
git branch

# How can i switch/change in new branches and change new branch 
git checkout neha-feat

# check branch
git branch

# how can create remote branch in local
git push --set-upstream origin neha-feat
