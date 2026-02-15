# DAT505_

#welcome to my repo




git <- "C:/Users/ADMIN/Desktop/DAT505/PortableGit/bin/git.exe"

system2(git, c("config", "--local", "commit.gpgsign", "false"))

system2(git, c("config", "--local", "--unset", "gpg.program"))
system2(git, c("config", "--local", "--unset", "user.signingkey"))

system2(git, c("config", "--local", "--get", "commit.gpgsign"))

setwd("C:/Users/ADMIN/Desktop/DAT505")

system2(git, c("config", "--show-origin", "--get-all", "commit.gpgsign"))

system2(git, c("config", "--show-origin", "--get-all", "gpg.program"))
system2(git, c("config", "--show-origin", "--get-all", "user.signingkey"))
system2(git, c("config", "--show-origin", "--get-all", "commit.gpgsign", "--global"))

setwd("C:/Users/ADMIN/Desktop/DAT505")
git <- "C:/Users/ADMIN/Desktop/DAT505/PortableGit/bin/git.exe"

system2(git, c("add", "-A"))

system2(git, c("commit", "--no-gpg-sign", "-m", "Update README / draft fixes"))

getwd()

setwd("C:/Users/ADMIN/Desktop/DAT505/DAT505_")
list.files(all.files = TRUE)

git <- "C:/Users/ADMIN/Desktop/DAT505/PortableGit/bin/git.exe"
system2(git, "status")

