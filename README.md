# Static Web Server
[Static Web Server](https://github.com/m3ng9i/ran)



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


## Nodejs        

```      
npm install -g http-server        
http-server -p 8000        

```        




## caddy        

`caddy -port 8000`        

`caddy browse`        













## Rust        

```        
cargo install https        
http        

```        









































