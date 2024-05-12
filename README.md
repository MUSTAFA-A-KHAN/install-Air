## Installing Air

If you prefer using a script for Air installation, then this repository can help. You can use the installation script provided by Air by running the following command:

```bash
curl -sSfL https://raw.githubusercontent.com/cosmtrek/air/master/install.sh | sh -s
```

This command will download and execute the installation script, which will install Air on your system.

Next, you need to add the path of the Air executable, which is located inside `./bin`, to your environment variable:

```bash
export PATH=$PATH:$(pwd)/bin
```

You can test whether Air has been successfully installed by entering the command:

```bash
air -v
```

This will result in:

```
  __    _   ___  
 / /\  | | | |_) 
/_/--\ |_| |_| \_ 1.52.0, built with Go 1.22.2
```

Now you're ready to use Air for your projects.
