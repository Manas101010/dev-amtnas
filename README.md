Yoo dude!
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Experiment no-6 ke lia following steps ==> Idhar image creation karna hai EXPERIMENT 6
Create a new folder 
Open in VS-Code
terminal chalu karo
git clone https://github.com/Manas101010/docker-starter.git(idhaar aap repo link)
uske cd into docker-starter
create a file named dockerfile or Dockerfile in that file add this code
[FROM node:18-alpine
WORKDIR /app
COPY . /app/
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000]
SQUARE BRACKET REMOVE KARDENA
uske baad save 
Image creation syntax==> docker build -t <image-name> . 
Image running kelia ==> docker run -d 127.0.0.1:3000:3000<image-name>
To check this docker ps for containers and docker images for docker images toh woh image dikhegi
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Experiment no -7 Isme hamko contarization ke steps follow karne hai  EXPEIRMENT 7
For this experiment we need to build a image toh either aap aapni ek image banao and then uspe yeh kaam karo OR
A image is created by default i.e redis
toh u can do 
docker pull redis [image bangyi abb redis naam ki iske baad docker ps and image kardena]
docker run - d redis [image run karne ke lia ]
docker ps kar lena 
For contarization there are two commands start and stop ok dono ke lia we need container id
docker ps kar container id select karo 
then type docker start/stop <container id paste karo>
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Experiment 6-7 ke lia docker app kholna padega but for experiment 8 docker hub kholna padega EXPERIMENT 8
Experiment 8 mai push and pull use karna hai right toh we need a repositary
first we do is 
docker tag redis USERNAME/repo-name:v1.0
docker tag redis username ki jagah ritesh ka username and repo-name as us wish kar dena but sab small hona chaiye
phir se docker ps and images karna
then docker push USERNAME/repo-name:v1.0 {redis ke baad wala part}
phir docker hub pe jake dikha dena repo
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Jenkins mai free project EXPERIMENT -4 
configure pe click then free project naam select git aur jo koi ek git pe repo hoga uska code lelena 
bas sab waise hi rehne dena koi bhi daal dena git link [https://github.com/Manas101010/DevOps-1exp2.git]
Apply and save 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Jenkine Pipeline mai Configure and then pipeline ke lia aarya wala jenkins repo fork ki thi uski repo ka link lelo EXPERIMENT 5
Default Pipeline script hota hai in usko SCM kardena 
SCM mai GIT isme jenkins deploy wali link use karna https://github.com/Manas101010/jenkins_deploy.git
git repo mai wo link daal dena branch mai main kar dena and create button click kar dena
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
For git wale thing since it will be used by other toh hamko make sure karna hai ki hamara hi git use hoo 
for that regardless what git experiment aaye we need to do this
git config --list [pehle wale user aajayenge]
git config --global user.name "amatbohra"{username dalo }
git config --global user.email ""{git wala mail dalo}
phir git commands bhagwan janne
EXPERIMENT 3 -----------------> Branching=> pehle ek naya se folder bana lena usme ek html file
git init [INITIALIZE EMPTY GIT]
git checkout -b new-branch-name [ADD A NEW BRANCH]
git add . [ADD FILES]
git commit -m "Your commit message" [COMMIT MESSAGE]
git push origin new-branch-name [WO WALI BRANCH KA PUSH]
EXPERIMENT 2 ----------------> AND 1 nhi malum 😭
