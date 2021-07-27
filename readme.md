#github bilan ishlash

1. Github.com saytidan ro'yxatdan o'tiladi
2. Kompyuterga github desktop va gitbash dasturlari yulab olinadi 
3. Github sozlamalarini o'rnatish

git config sozlamalari listi
```bash
git config --list
```

git foydalanuvchi ismi va email
```bash
git config user.name
git config user.email
```

git sozlamalarini o'rnatish
```bash
git config --global user.name "Ismingiz"
git config --global user.email example@mail.com"

```

4. Git repository (git yangi papka-loyiha)

	- Dastlab github.com saytida yangi repository ochib olamiz
	
	- keyin kompyuterimizda joylashgan loyihamizni _gitbash_ orqali ochamiz

	- loyihani initalizatsiya qilish
	```bash
		git init
	```

	- Loyiadagi fayllarni qo'shih
	```bash
		git add .
	```

	- Loyihaga dastlabki commit ni qo'shish 
	```bash
		git commit -m "first commit"
	```

	- branch ni nazorat qilish
	```bash
	git branch -M main	
	```

	- githubdagi loyihani ulash 
		bu yerda:
		 _username_ - github login
		 _projectname_ - loyihani githubdagi manzili
	```bash
		git remote add origin https://github.com/username/projectname.git
	```

	- loyihani yuklash
	```bash
		git push -u origin main
	```

	Yuqoridagi amallar loyiha(repository)ni github yuklab berishni ta'minlaydi.

	- Loyihani statusini ko'rish (yangi fayllarmi bormi yoki yo'qligini fayllarda o'zgarish bor yoki yo'qligini tekshiradi)
	```bash
	git status
	```