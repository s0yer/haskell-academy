
ghcpu install

https://www.haskell.org/ghcup/

powerShell:
Set-ExecutionPolicy Bypass -Scope Process -Force;[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072;Invoke-Command -ScriptBlock ([ScriptBlock]::Create((Invoke-WebRequest https://www.haskell.org/ghcup/sh/bootstrap-haskell.ps1 -UseBasicParsing))) -ArgumentList $true

---------execute

ghc --make MathQuestion.hs

ghci MathQuestion.hs

./MathQuestion.hs

----

https://www.haskell.org/ghcup/steps/
