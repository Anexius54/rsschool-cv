# Evgeniy Sapronov

## Contacts

- Telegram: @hellatrigger69
- Email: ek.sapronov@gmail.com

## About

I graduated from SibSUTIS and now work as a system administrator. Now I want to gain frontend skills.

## Skills

- C/C++
- Python
- Git

## Code example
```C++
int createDaemon(char *ProcName) {
    int rv;
    char *arg[] = {ProcName, 0};

    switch(fork()) {
        case -1:
            perror("fork");
            return 1;
        case 0:
            setsid();
            cout << "pid: " << getpid() << endl;
            cout << "ppid: " << getppid() << endl;
            chdir("/");
            fclose(stdin);
            fclose(stdout);
            fclose(stderr);
            execv(arg[0], arg);
        default:
            wait(&rv);
    }

    return 0;
}
```
## Languages

- Russian (native)
- English (A2)

## Education
Siberian State University of Telecommunications and Information Science
