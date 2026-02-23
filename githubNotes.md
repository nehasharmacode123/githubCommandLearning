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

