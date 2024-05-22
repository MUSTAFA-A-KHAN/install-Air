# Air Installation
1. Sessional
2. Global

## Sessional Installation

If you prefer using a script for Air installation, then this repository can help. You can use the installation script provided by Air by running the following command:

If you don't have curl installed 

```bash
sudo apt install curl
```

Download the sh file

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

## To install Air globally, you can follow these steps:

1. **Download the installation script** to a local file named `install_air.sh`:

    ```bash
    curl -sSfL https://raw.githubusercontent.com/cosmtrek/air/master/install.sh -o install_air.sh
    ```

2. **Execute the installation script**, placing the Air executable in `/usr/local/bin`:

    ```bash
    sudo sh install_air.sh -b /usr/local/bin
    ```

    This command will execute the script with elevated privileges (`sudo`) and install Air globally by placing the executable in `/usr/local/bin`, which is typically in the system's PATH.

3. After following these steps, **Air should be installed globally** on your system, and you can verify the installation by running:

    ```bash
    air -v
    ```

    This should display the version information of Air if the installation was successful.






