# BASIC TERMS

`repo` container for a project you want to track with git

`commits` like save points for the project

`branches` new/seperate version of the main repo. yani bir şeyleri test ediyorsak, yeni şeyler deniyorsak yeni, daha izole bir ortam oluşturmak daha mantıklı olur bu yüzcen main branch üzerinden yeni bir branch yaparız. yeni bir branchte main branchteki kodu kopyalar ve üzerinde çalışılır. her şey okeyse main branchle merge edebiliriz.  

## three key areas

* modified: files are changed but not committed yet(yani hala working aşamasında herhangi bi kaydetme yok, YAAAANİ oyunu oynuyosun şuan)
* staged: marked modified file for commiting in its current version for the next snapshot  
* committed: chosen files are committed. yani değişikliklerin database e kaydedildi. git directorynde permanently o savepoint(snapshot) store ediliyor

## undoing things

* checkout commit: go back to code in that snapshot. dont make any difference in commit history
* revert commit: undone the specific commit. makes a new commit that reverts anything done in that commit. commit historyde bir şey değişmez
* reset commit: kullanma ignore et kullanmana gerek bi durum yok. commit historyyi de alter eder tehlikeli  

## making branches

launch edilen branch çoğunlukla main branch. değişiklik / yeni şeyler deneme yeri de branchler. birden fazla branch olabilir collab yaparken de handy bir şey ama şöyle bi `conflict` var: ben mainden bir branch çıkardım ve bir takım değişiklikler yaptım. bunları da sonrasında tekrar maine merge etmek istedim; fakat bu sırada biri mainden bir değişiklik yapmış. bu durumda git conflict uyarısı verir. buna dikkat etmek gerekiyor.

## making collabs

before starting the branch make sure you have the latest vers of the master branch. dont merge it the master branch immediately. instead push the branch. then make a pull request to repo so the team can agree or not. if all is ok you can merge pull req
