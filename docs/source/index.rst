Welcome to Lumache's documentation! Kiểm tra file doc
===================================

1. Cài đặt môi trường
1.1.	Cài đặt chocolatey on windows 11
B1: Mở PowerShell bằng Administrator
B2: Chạy lệnh : Get-ExecutionPolicy
B3: Run: Set-ExecutionPolicy AllSigned
B4: Run: Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
1.1.	Cài đặt yarn
Cài yarn thì yêu cầu cài thêm Nodejs version 16.x.x
-	Run: choco install nodejs-lts
-	Run: choco install yarn
-	Cài thêm go language và tdm64 build GCC
1.2.	Build source code
Fontend
-	Run: yarn install --immutable
-	Run: yarn start
Backend
-	Run: make run (cần cài đặt make và run bằng git bash). Chưa fix được chạy bằng cmd hay powershell

Link tham khảo: https://github.com/grafana/grafana/blob/main/contribute/developer-guide.md

II. Import/Export Dashboard
Import: Từ dashboard có sẵn chọn share -> export -> savefile json
Export: Tạo new dashboad -> chọn import file json
Chú ý: Kiểm tra add datasource và các panel thêm trước

III. Deploy trên server



Check out the :doc:`usage` section for further information, including
how to :ref:`installation` the project.

.. note::

   This project is under active development.

Contents
--------

.. toctree::

   usage
   api
