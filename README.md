rails-vagrant

=============

## Getting Started !

### 環境構築
- virtualboxを下記URLからインストール

  http://download.virtualbox.org/virtualbox/5.1.12/VirtualBox-5.1.12-112440-OSX.dmg

- Vagrantを下記URLからインストール

  https://releases.hashicorp.com/vagrant/1.9.1/vagrant_1.9.1.dmg

- Vagrantのプラグインをインストール

  ```
  $ vagrant plugin install vagrant-vbguest
  ```

#### 下記はローカルで行う手順です
- このリポジトリをクローンする

  ```
  $ git clone https://github.com/rabichan/rails-vagrant.git
  ```

- クローン先のディレクトリに移動する

  ```
  $ cd ~/rails-vagrant
  ```

- vagrantを起動する

  ```  
  $ vagrant up
  ```  

- centosの中に入る

  ```  
  $ vagrant ssh
  ```  

#### 下記はvagrant内で行うコマンドです。
- vagrantディレクトリに移動する

  ```  
  # varantディレクトリ配下に置くと、localのプロジェクトとsyncしてくれるため.
  $ cd /vagrant
  ```  

- railsプロジェクトを作成する
  ```  
  $ bundle exec rails new sample
  ```  

- railsアプリを起動する
  ```  
  $ bundle exec rails s -b 0.0.0.0
  ```  

## About this app

### Version
 - ruby: 2.3.3
 - rails: 4.2.5.2
