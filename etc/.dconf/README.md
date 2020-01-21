# .dcfg
Global debian config repo

Source: https://www.atlassian.com/git/tutorials/dotfiles
========================================================

Howto:
sudo groupadd config
sudo usermod -a -G config <username>
sudo mkdir /etc/.dcfg
sudo chown -R root.config /etc/.dcfg
sudo chmod -R 2775 /etc/.dcfg/
      #git init --bare /etc/.dcfg
git clone https://github.com/Beliaal/.dcfg.git /etc/.dcfg
alias config='/usr/bin/git --git-dir=/etc/.dcfg/ --work-tree=/'
config config --local status.showUntrackedFiles no
#echo "alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'" >> $HOME/.bashrc


Work in progress
