## Contents
<details><summary>Language</summary>
<p>

* **[Go](#Go)**<br />      
* **[Python](#Python)**<br />        
* **[Ruby](#Ruby)**<br />        
* **[Perl](#Perl)**<br />        
* **[Nodejs](#Nodejs)**<br />
* **[Rust](#Rust)**<br />        






</p>
</details> 

# Go        

## caddy        

`caddy -port 8000`        

`caddy browse`       

## Ran

[Static Web Server](https://github.com/m3ng9i/ran)

```      
wget https://raw.githubusercontent.com/vpslinuxinstall/StaticWebServer/master/ran_linux_386.zip       
unzip ran_linux_386       
chmod +x ran_linux_386        
./ran_linux_386 -p 8000 -i index.html        

```
       



## Algernon        

[algernon](https://github.com/xyproto/algernon) 

```        
wget https://github.com/vpslinuxinstall/StaticWebServer/raw/master/algernon.zip        
unzip algernon.zip      
cd algernon     
cp algernon path/to/the/index.html      
cd path/to/the/index.html
chmod +x algernon        
./algernon -x 8000        

```        

    


















# Python        

`python -m SimpleHTTPServer 8000`        

`python3 -m http.server 8000`        

## twistd        

```        
git clone https://github.com/crossbario/autobahn-python        
cd autobahn-python        
pip install -e .[twisted]        
twistd -n web -p 'tcp:port=8000' --path .        

```        

```        
wget https://raw.githubusercontent.com/vpslinuxinstall/StaticWebServer/master/autobahn-python-19.10.1.zip        
unzip autobahn-python-19.10.1.zip        
cd autobahn-python-19.10.1.zip        
pip install -e .[twisted]        
twistd -n web -p 'tcp:port=8000' --path .        

```

# Ruby        

`ruby -run -ehttpd . -p8000`        

## adsf        
```        
gem install adsf        
adsf -p 8000        

```        
There is no ftp server.        


# Perl        

## Plack        

```        
cpan Plack        
plackup -MPlack::App::Directory -e 'Plack::App::Directory->new(root=>".");' -p 8000        

```        




## Brick        

```        
cpan HTTP::Server::Brick        
perl -MHTTP::Server::Brick -e '$s=HTTP::Server::Brick->new(port=>8000); $s->mount("/"=>{path=>"."}); $s->start'        

```        








## SimpleHTTPServer        

```        
cpan App::SimpleHTTPServer        
serve_dir        

```        


# Nodejs        

## http-server         

```      
npm install -g http-server        
http-server -p 8000        

```        



       













# Rust        

## https

```        
cargo install https        
http        

```        












[And more](https://gist.github.com/willurd/5720255#comment-841915)     


[And more](https://github.com/imgarylai/awesome-webservers)     







































