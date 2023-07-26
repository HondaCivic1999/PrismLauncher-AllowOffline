# Prism Launcher - Allow Offline Version

## Notes
When making an offline account, `AccountListPage::on_actionAddOffline_triggered()`  located in `launcher/ui/pages/global/AccountListPage.cpp` checks if you already have an account, and if you don't, it prematurely returns from the account creation.

We can allow offline account creation without a real account by making the account check not exit the method prematurely or by just removing the whole `if` statement.

## Legal Disclaimer
You should probably buy Minecraft legally since this breaks their EULA. Or don't, who cares.
