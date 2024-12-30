```bash
pip install -r requirements.txt 
```

FastAPI in Azure Functions v2:
https://learn.microsoft.com/en-us/samples/azure-samples/fastapi-on-azure-functions/fastapi-on-azure-functions/



node@20 is keg-only, which means it was not symlinked into /opt/homebrew,

because this is an alternate version of another formula.

  

If you need to have node@20 first in your PATH, run:

  echo 'export PATH="/opt/homebrew/opt/node@20/bin:$PATH"' >> /Users/heiko/.bash_profile

  

For compilers to find node@20 you may need to set:

  export LDFLAGS="-L/opt/homebrew/opt/node@20/lib"

  export CPPFLAGS="-I/opt/homebrew/opt/node@20/include"

==> **Summary**

🍺  /opt/homebrew/Cellar/node@20/20.18.1: 2,068 files, 58.7MB

==> **Running `brew cleanup node@20`...**

Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.

Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).