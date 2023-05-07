# Docker_lab6

Zainstalowałem buildkita zgodnie ze skryptem laboratorium
![image](https://user-images.githubusercontent.com/83607788/236684251-5cd49bf0-1e11-496e-8899-a65f6d6713d6.png)
![image](https://user-images.githubusercontent.com/83607788/236684364-57243e46-aedb-4688-afc2-bf141287a262.png)
Uruchomiłem kontener buildkit
![image](https://user-images.githubusercontent.com/83607788/236684411-90f00611-7e63-4173-aef2-4a7055bec52a.png)
![image](https://user-images.githubusercontent.com/83607788/236685113-eedcce04-ee8c-482e-a89e-2e641e69c3da.png)

buildkit nie chce działać
![image](https://user-images.githubusercontent.com/83607788/236684644-1c6b7f1b-ea36-4e78-ab0c-ceb4de8025fd.png)

![image](https://user-images.githubusercontent.com/83607788/236684842-03d8a42e-3cce-497c-9df6-aaee53b4b2e2.png)


buildctl build --frontend=dockerfile.v0 --local context=. --local dockerfile=. --output type=image,name=docker.io/lukas5555510/lab6repo:test1,push=true
[+] Building 0.0s (0/0)
error: listing workers for Build: failed to list workers: Unavailable: connection error: desc = "transport: error while dialing: dial unix /run/buildkit/buildkitd.sock: connect: no such file or directory"

próbowałem restartowac buildkita
![image](https://user-images.githubusercontent.com/83607788/236685479-46162466-2a9e-4327-88d6-ba2b71f7c701.png)

Ale gdy przeczytałem co ten błąd oznacza zaniechałem dalszego działania
