# Tare — Privacy Policy

**Last updated: 25 September 2026**

Tare is a personal finance app for iPhone, iPad and Mac. This policy says what
happens to your information, in plain words. Where the answer is "nothing leaves
your device", it says so, because for most of what Tare does that is the truth.

## The short version

- **If you use only Tare's free features, Tare sends nothing to us. Ever.** There
  is no account to create, nothing to log in to, and no server of ours involved.
  No paid feature is available yet, so today that is true for everyone.
- **We do not track you, and Tare collects no analytics.** No advertising
  identifiers, no third-party analytics SDKs, no profiling. What Apple can pass
  to us, if you allow it, is under *What Apple passes to us*.
- **We never sell your information**, and we never share it for advertising.
- **We never see your bank username or password.** Nobody at Tare can, by design.

## What Tare does on your device

Reading receipts, recognising text, categorising a purchase, totalling a month,
detecting a recurring charge and writing advice all run **on your iPhone, iPad or
Mac**. None of it involves a network request.

- **Receipt photographs** are read on the device. The photograph you keep with a
  receipt stays on the device you saved it on: Tare does not upload it, and does not
  sync it to your other devices. Like everything an app keeps on your device, it
  is part of that device's backup if you make one (see *Your device's backup*).
- **Finding receipts in your photo library** is optional and off by default. When
  you turn it on, Tare looks at photos on that device only. It keeps a list of the
  photos that looked like receipts, with what became of each and when, and a
  note of how far through your library it has got. It never keeps anything it
  read from a photo. That list stays on the device: it does not sync, and it is
  left out of the device's backup.
- **Card numbers are cut from the text Tare stores.** In the text Tare reads from
  a receipt, and in the comment column of a file you import, any long run of
  digits that could be a card number is cut to its last four before it is saved.
  That text keeps those four digits whatever the payment method; a transaction's
  own card field keeps them only when it was paid by card or wallet, or the
  method is unknown. The other columns of an imported file, such as the place,
  the sheet's name and the transfer column, are kept as the file has them. This
  is done to text, not to the photograph: the picture Tare keeps shows the
  receipt as it was photographed, so if the paper shows a full card number, so
  does the picture. Tare does not scan text you type yourself, such as a note
  you write.

## Sync through your own iCloud

If you are signed in to iCloud, your ledger syncs between your own devices using
Apple's CloudKit, in **your** private iCloud database. We have no access to it —
it is your Apple account, not ours, and Apple bills the storage to you.

Your personal details in that database are **end-to-end encrypted**, so they are
unreadable even to Apple: merchant names, notes, tags, the last four digits of a
card, transfer counterparties, receipt text and addresses, account names, account
numbers' last digits, institution names, category names and rule values. The rest is encrypted by
Apple but not end-to-end: amounts, currencies, dates, how you paid (card, cash
and so on), the type of each account, category icons, whether a transaction was
typed, scanned or imported, how each rule matches, and the app's own identifiers
and flags. That was our choice, not a limit of CloudKit: without the names beside
them these say little, and if your iCloud Keychain is ever reset you lose the
synced copy of every end-to-end encrypted detail, which should not include your
figures.

## Your device's backup

Tare's data on your iPhone, iPad or Mac — your ledger and any receipt
photographs — is part of that device's backup, exactly as every app's data is, if
you back it up: to iCloud or a computer for an iPhone or iPad, with Time Machine
for a Mac. Apple encrypts iCloud Backup, but it is
**end-to-end encrypted only if you turn on Advanced Data Protection** for your
Apple account; otherwise Apple holds the keys to it. The end-to-end encryption
described in the section above applies to Tare's sync database, not to your
device's backup. Tare cannot see either.

## What Apple passes to us

If you have chosen, in your device's settings, to share analytics with app
developers, Apple passes us crash reports and aggregated usage figures. If you
test Tare through TestFlight and send feedback, we receive what you send: your
comment, any screenshots, your device model and system version, and any crash
report you choose to send. We use it to fix the app, and copies we download to
do that are deleted afterwards.

## If you connect a bank (a paid feature, not available yet)

**Connecting a bank is not available yet**, and nothing in this section happens
in the app today. It says how it will work, so you can judge it before it
arrives, and this policy will be updated before it does. It will be optional and
part of a paid subscription. Paid features are the only parts of Tare that
involve our servers.

- **You sign in with Apple first.** Connecting a bank needs an account on our
  servers so the connection belongs to you. Tare uses Sign in with Apple and does not ask
  Apple for your name or your email address. We store the identifier Apple gives
  us for Tare. If Apple includes an email address anyway, we keep it too,
  encrypted under a key unique to you. For each device you sign in on, we also
  keep a random identifier Tare makes for that device, the word "iPhone" or
  "Mac" (never your device's own name), and when that sign-in started and when
  it ends. Deleting your account deletes all of this, and disconnects any bank
  first. It does not yet remove Tare from the apps using Sign in with Apple in
  your Apple Account settings; you can remove it there yourself.
- **Your bank credentials never reach us.** The connection is made through
  **Plaid**, whose own screen collects them; they travel from your device to
  Plaid and never through Tare. We receive a token that lets us read
  transactions, and nothing that could let anyone sign in to your bank.
- **We request read access only**: your accounts, their balances and their
  transactions. Not the ability to move money.
- **What we store**: the access token and your bank's name, encrypted under a
  key unique to you; each account's name, type, last four digits and balance;
  and the transactions we read, with their merchant names and notes encrypted
  under your key. Amounts, dates and account names are not encrypted under your
  key. We keep them so they can be matched against receipts you have already
  entered and not counted twice.
- **You will be able to disconnect at any time**, in the app. Disconnecting
  revokes the token with Plaid, so it can no longer be used to read your bank.
  The accounts and transactions already read stay with your account until you
  delete it.
- Plaid has its own privacy policy, at plaid.com/legal.

## Written advice and harder receipts (paid features, not available yet)

Neither exists in the app today; this says how they will work. Written advice
from a language model will send our server a summary of the figures it describes
(amounts, categories, dates) and any question you type about your spending.
Reading a receipt your device could not will send that receipt's text. Our
server will pass these to Anthropic, whose model writes the reply. Your receipt
photographs are never sent. The advice Tare gives today is written on your
device.

## What we keep, and for how long

- Free tier: nothing, because the app sends us nothing.
- Paid tier: what is listed above, until you delete your account. Ending a
  subscription does not delete your account or what we hold; Delete Account, in
  the app, does. It removes everything from our live database at once, after
  disconnecting any bank. Copies in our database backups remain until those
  backups expire.
- Delete all data, in Settings, erases your ledger on this device and, if it
  syncs through your iCloud, on your other devices too. Receipt photographs do
  not sync, so it removes only the photographs this device kept for the receipts
  it erased; photographs kept on your other devices are not removed by it.
  Deleting the Tare app from an iPhone or iPad removes the photographs it kept
  there. Delete all data does not touch an account on our servers.
- Like any server, ours sees the internet address each request comes from. It
  uses it only to limit how often it can be called, holding it in memory for a
  minute at a time and never writing it down; the
  company that hosts our server may keep it in its own logs. Our own logs note
  when an account is created, signs in or out, or is deleted, by an account
  number, never by name.
- Our servers do not keep an audit log yet; this policy will be updated before
  they do.

## Children

Tare is not directed at children under 13 and we do not knowingly collect their
information.

## Your rights

Wherever you live, you can ask what we hold, ask for a copy, ask for it to be
corrected, or ask for it to be deleted. If you have never signed in to Tare, the answer
to the first question is "nothing", apart from any feedback you chose to send
through TestFlight. Export of your own ledger is built into the
app, as CSV, and needs no request.

## Changes

If this policy changes in a way that affects what happens to your information, the
date at the top changes and the new version is published here before it takes
effect. The app downloads no instructions of its own, so a change in what it sends can
only reach you in an app update.

## Contact

Tareque Rishad — tareque.rishad@gmail.com
