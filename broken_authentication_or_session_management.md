# Broken authentication or session management

### Password reset link does not expire

1. You create an account in example.com. You add email a@email.com
2. Your email account gets hacked.
3. The hacker figures out you have a user on example.com. The hacker clicks the reset-password-link. But does not use it.
4. The hacked person figures out that he is hacked and thus goes to example.com to change his password.
5. The hacker now clicks on the link and manage to reset the password.  

The problem here is that the first reset-link should be blocked once the second is sent.

#### Relevant bug bounty reports
https://hackerone.com/reports/23579
