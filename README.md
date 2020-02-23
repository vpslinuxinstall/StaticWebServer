## Contents
<details><summary>Language</summary>
<p>

* **[Go](#Go)**<br/> 
       * **[server](#server)**<br />
       * **[caddy](#caddy)**<br />
       * **[Ran](#Ran)**<br />
       * **[Algernon](#Algernon)** <br />
       * **[Spark](#Spark)**<br />
* **[Python](#Python)**<br />
       * **[twistd](#twistd)**<br /> 

* **[Ruby](#Ruby)**<br /> 
       * **[adsf](#adsf)**<br /> 
* **[Perl](#Perl)**<br /> 
       * **[Plack](#Plack)**<br />
       * **[Brick](#Brick)**<br />
       * **[SimpleHTTPServer](#SimpleHTTPServer)**<br />
* **[Nodejs](#Nodejs)**<br />
       * **[http-server](#http-server)**<br />
* **[Rust](#Rust)**<br /> 
       * **[https](#https)**<br />






</p>
</details> 

# Go        

## server      

[server](https://github.com/jpillora/serve/)

## caddy        


```        
caddy -port 8000        
caddy browse        

```
      

## Ran

[ran](https://github.com/m3ng9i/ran)

```        
go run github.com/m3ng9i/ran -p 8000 -i index.html  -r path/to/the/index.html       

```

```        
wget https://github.com/vpslinuxinstall/StaticWebServer/raw/master/ranSource.zip        
unzip ranSource.zip        
cd ran-master             
go run ran.go -p 8000 -i index.html  -r path/to/the/index.html        

```        






```      
wget https://raw.githubusercontent.com/vpslinuxinstall/StaticWebServer/master/ran_linux_386.zip       
unzip ran_linux_386     
cd ran_linux_386     
cp ran_linux_386 path/to/the/index.html        
cd path/to/the/index.html
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

 ## Spark       
 
 [Spark](https://github.com/rif/spark)       
 
 ```        
 go run github.com/rif/spark -port 8000      
 
 ```
 
 ```       
wget https://github.com/vpslinuxinstall/StaticWebServer/raw/master/sparkSource.zip       
unzip sparkSource.zip       
cd sparkSource       
cp spark.go path/to/the/index.html        
cd path/to/the/index.html        
go run spark.go -port 8000        
 
 ```        
 
 ```        
wget https://github.com/vpslinuxinstall/StaticWebServer/raw/master/spark_1.7.3_linux_386.zip        
unzip spark_1.7.3_linux_386.zip        
cd spark_1.7.3_linux_386        
cp spark path/to/the/index.html        
chmod +x spark        
./spark -port 8000        

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

[Filebrowser](https://github.com/vpslinuxinstall/Filebrowser)       

[Directory Lister](https://github.com/vpslinuxinstall/Directory-Lister)      

[dzzoffice](https://github.com/vpslinuxinstall/dzzoffice)

[dzzoffice](https://github.com/vpslinuxinstall/CloudDzzOffice)      

[Kodexplorer](https://github.com/vpslinuxinstall/Kodexplorer)      

[h5aiwebftp](https://github.com/vpslinuxinstall/h5aiwebftp)        



























































