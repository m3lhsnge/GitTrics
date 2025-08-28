###### **Terminal Komutları**

cd ➤ *bulunan konumu değiştirme*

ls ➤ *listeleme*

pwd ➤ *mecvut konumu gösterme*

rm -r ➤ *klasörü siler*

rm -rf ➤ *içi dolu klasör silme*

rm dosya.uzantı ➤ *dosya silme*

touch dosya.uzantı ➤ *dosya oluşturur*

mkdir ➤ *klasör olusturur*

mv dosya.uzantı klasör/ ➤ *dosyayı klasöre taşır(dosya adına boşluk varsa "" içinde yaz)*

lsDesktop ➤ *desktoptaki dosyaları listeler(benim özel desktop için komutlarım normalde ls/cd desktop çalışır)*

cdDesktop ➤ *desktopun içine girer*



#### Github İçin Komutlar



git config --global user.name "user\_name" ➤ git bash'in en başında gereken githubtaki isimle aynı olması gereken kullanıcı adı

git config --global user.email "user\_email" ➤  git bash'in en başında gereken githubtaki ile aynı olması gereken email



git init  ➤ .git oluşturma 

git add . ➤ stage bölgesine dosyaları ekleme takip etme

git commit -m "..." ➤ repoyu mesajla ekleme

git status ➤ mevcut durumu görüntüleme

git commit -am ".." ➤ bütün dosyalar takip ediliyorsa hepsini repoya ekler

git commit --amend -m "..." ➤ commmit mesajını ve stage bölgesindeki bütün değişikleri son commite ekler

git restore --stage <file> ➤ yapılan değişiklik stage den kaldırılır

git restore --stage . ➤ ile hepsi stageden çıkarılır

(ilk stage e alınır sonra commit yapılır)

git log ➤ reponun geçmiş commitleri gözükür

git log --oneline ➤ kısaltılmıs geçmiş



➤.gitignore dosyası oluşturup içine görünmesini istenmeyen dosyaları ekleyerek görünmesini engeller klasör için <file\_name>/ ile klasörü görmez

➤\*./dosyaformatı gitignore içine yazılırsa bu türdekiler görünmez 

git rm --cached <file\_name> ➤ ile sonradan gitignore dosyasına yazılan ancak takip edilen dosya artık takip edilmez

git rm --cached r <klasör\_ismi> ➤ ile klasörü cache den çıkarır

git mv <dosya ismi> <dosya ismi> ➤ dosyanın isim tür değiştirmesini sağlar

git mv <dosya ismi> <klasör ismi/> ➤ dosyayı klasöre taşır



branch master la başlar adını 'main' olarak değiştirmek önemli github için

git branch ➤ branchi gösterir ilk basta main (master) branch içinde olursun

git branch <branch\_ismi> ➤ branch olusturur

git switch <branch\_ismi> ➤ branchler arası geçişi sağlar

diğer branchlerde yapılan commit işlemleri diğer branchlere eklenmediği sürece etki etmez

git switch -c <branch\_ismi> ➤ branch oluşturup ona geçiş yapar

git switch -f <branch\_ismi> ➤ diğer branche zorla geçer eğer bir branchte düzenleme yapıp commit etmeden diğerine geçmeye çalışırsak hata alırız çünkü iki aynı dosya çakışabilir bu durumda bu komutla değişikliklerin kaybolması haliyle diğer branche geçer

git branch -m <isim> ➤ git switch ile geçilen branchin adını değiştirmeye yarar

git branch -d <isim> ➤ branchi siler ancak silenecek branch içinde olunmaması gerekir

git merge <isim> ➤ olduğun branchle diğer branchi birleştirir

git stash ➤ commitlenmeyen değişiklikleri stash ile kaydedip gizlemeye yarar

git stash ➤ pop gizlenen değişiklikleri ortaya çıkarır

git stash list ➤ stash ile gizlenen ögeler listelenir

git checkout <commit hash'i> ile istenilen commite gidilir ancak 'main/master' son commiti gösterirken 'head' gidilen commiti gösterir bu durumda 

1.Seçenek, git switch master/main ile mastere geri dönülür değişiklikler aynı kalır

2.Seçenek, gidilen committeyken git branch (isim) ile yeni bir branch açılıp buradan branche devam edilebilir git switch master ile mastere dönülürse değişiklikler aynı kalır

git reset <commit hashi> ➤ seçilen commit sonrası commitleri siler ancak yapılan değişiklikler kalır

git reset --hard <commit hashi> ➤ seçilen commit sonrası commitleri içerikleriyle siler

git revert <commit hashi> ➤ seçilen committe yapılan değişiklikler geri alınır ancak commit logda kalır ve bu committen sonra yeni bir commit atılarak önceki commitin revert edildiği belirtilir

git diff ➤ yapılan değişiklikleri gösterir

git diff <commit hashi> <commit hashi> ➤ commitler arasında yapılan değişiklikleri gösterir

git diff <branch ismi> <branch ismi> ➤ branchler arasında yapılan değişiklikleri gösterir

git rebase ➤ merge edilen commitler arasındaki merge commit loglarını temizler ancak tarihi baştan sırayla yazacağından karışıklık çıkarma olasılığı vardır(MÜLAKATLARDA SORULUR BAYA)



git remote add origin <repo linki> repoyu bağlamaya yarar

git push -u origin main commitleri repoya pushlar

git push bu komutlardan sonra direkt commitleri pushlamaya yarar	









