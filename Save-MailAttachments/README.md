# Connect to your mailbox using IMAP and save all attachments locally

## Import
To import this cmdlet, `cd` to the directory where `Save-MailAttachments.ps1` is kept and execute the following: \
\
`Import-Module .\Save-MailAttachments.ps1`

## Parameters
`-IMAPServer` - accepts target imap server name. *REQUIRED* \
`-Username` - accepts target mailbox address. *REQUIRED* \
`-Password` - accepts target mailbox password. *REQUIRED* \
`-Port` - accepts IMAP connection port. *REQUIRED* \
`-TargetPath` - accepts directory, where attachments will be saved. *REQUIRED* \
`-DeleteFromInbox` - specify if you want to delete emails with attachments from inbox. *REQUIRED*


## Usage

To download attachments locally:
`Save-MailAttachments -IMAPServer imap.yandex.ru -Username 'username@yandex.ru' -Password 'password' -Port 993 -TargetPath 'C:\Temp\'`

To download attachments locally and delete emails with attachments from Inbox:
`Save-MailAttachments -IMAPServer imap.yandex.ru -Username 'username@yandex.ru' -Password 'password' -Port 993 -TargetPath 'C:\Temp\' -DeleteFromInbox`
