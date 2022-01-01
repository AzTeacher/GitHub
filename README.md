# Windows əməliyyat sistemi üçün Git yüklənməsi

Git yükləmək üçün https://git-scm.com/download/win adresine gedirik.  
**Komputerinizin əməliyyat sisteminizinə uyğun olan -bit Git for Windows Setup** yükləmək üçün  qovluğunu yükləyirik.     
   
   
Quraşdırma faylını işə salırıq. Uyğun ayarlar istədiyimiz şekildədirsə **next** veya ayar dəyişikliyi etmək istədiyimizdə ayarımızı düzəldib **next** klik edirik.

**Adjusting your Path environment**    
Bu hissədə əmrlər sətirlərində unix əmrlərinin işləməsi üçün aşağıdakı hissəni seçirik.   
- [x] Use Git and optional Unix tools from the Command Prompt

Digər ayarları özümüzə uyğun ayarladıkdan sonra quraşdırmanı bitiririk.

**Git Ayarlarını Edək**   
Əmr sətirinə aşağıdakı ayarları edərək istifadəçi ayarlarını edək.
```sh
git config --global user.name "İstifadəçi adınız"
```

```sh
git config --global user.email "İstifadəçi mail adresi"
```
Global ayarlara nəzər yetirək.
```sh
git config --list --global
```

**Yaratdıqımız proyekti Github'a yükləyək**    
Qovluqumuza git'i əlave edək.

```sh
git init
```

Qovluqumuza stage'e ekleyelim
```sh
git add .
```

Qovluqumuzu commit edelim
```sh
git commit -m "first commit"
```
  
**Poyektimizi Github'a yüklüyək**   
Github səhifəsində new klik edərək yeni bir **repo** yaratmaqa başlıyaq.  
Repomuzun adını, görünüş tipini, ve diğer ayarlarını etdikdən sonra create repository klik edirik.
```sh
git remote add origin https://github.com/istifadəçi-adınz/reponuzun-adı.git
```
```sh
git branch -M main
```
```sh
git push -u origin main
```
Və sonda isə GitHub -da proyektimizi yeniləyirik buda son....
