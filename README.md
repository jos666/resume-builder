# resume-builder
自动生成简历


Build your own resume with `Ruby`. Clone this repo:

    git clone https://github.com/Diveinedu-CN/resume-builder.git

Update `config/resume.yml` with required data and replace `config/profile.png` with your photo. Now, run:

	./build.sh 

And you are done! 

##ruby install
1. 安装需要的组件
```
yum install openssl-devel -y
```

2. 安装ruby 2.0
```
wget ftp://ftp.ruby-lang.org/pub/ruby/2.0/ruby-2.0.0-p353.tar.gz
tar xvf ruby-2.0.0-p353.tar.gz 
cd ruby-2.0.0-p353
./configure --prefix=/usr/local/ruby
make
make install
```
3. 安装rubygems
```
wget http://production.cf.rubygems.org/rubygems/rubygems-2.0.7.tgz
tar xvf rubygems-2.0.7.tgz
cd ../
cd rubygems-2.0.7
ls
/usr/local/ruby/bin/ruby 
/usr/local/ruby/bin/ruby  setup.rb
```

4. 使用
```
export PATH=/usr/local/ruby/bin:$PATH
./build.sh

cd resume
python -m SimpleHTTPServer
```

浏览器打开 ip:8000
