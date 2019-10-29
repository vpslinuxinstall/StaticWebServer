# Static Web Server
[Static Web Server](https://github.com/m3ng9i/ran)



# Python        

`python -m SimpleHTTPServer 8000`        

`python3 -m http.server 8000`        

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

There is no ftp server.        



























