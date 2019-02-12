# mac-workstation-role
1. install homebrew: /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
2. brew install pipenv git
3. mkdir ~/git && cd ~/git && git clone https://github.com/jsermer/mac-workstation-role.git && cd mac-workstation-role
4. pipenv install
5. pipenv run ansible-galaxy install -r requirements.yml
6. pipenv run ansible-playbook -i inventory.yml setup_mac_workstation_playbook.yml -K

Inspiration was provided by https://github.com/geerlingguy/mac-dev-playbook
