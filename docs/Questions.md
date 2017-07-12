# Questions

1. Permissions - do we need a role-based system or do permissions need to be managed for each data/object type? (This really depends on what Ray thinks his user population will be like.)

We need 2 roles - admin, user

2. Contacts - should this be a free-form text field or do we need a database of contacts who are assigned to items?

Freeform text is fine

3. Notes - will Ray need to manage many notes about one item, or will he prefer to have a single notes field that gets edited over and over?

Single big freeform text field is fine

4. What about deleting sites, subnets, etc?

Yes - need to do this 

BUT NO CASCADING DELETES

Will need to understand what data is orphaned and show it somewhere.

5. Add filter/search options in the list views?

Yes, Ray likes search!

6. Will all data need to be updated at the same frequency, or will (for example) the notes be updated far more often than contacts or site name/address? Would adding/editing notes with one click be a good UX approach?

Notes are not updated frequently.

7. Okay if view and add forms are in modals over the list screens?

Okay.

8. Can Ray help us develop a small set of realistic test data to use?

Yes, he can do that.

9. Are we only managing V4 data, or are we going to need to manage V6, too?

IPV4 only.

10. On average, how many subnets are associated with a site?

Maybe up to 20.

11. For non-admin users, do we restrict what sites/subnets are listed? We know that we will suppress the add/edit buttons, but are unclear about initial data filtering.

12. What are our design goals? (Colors, fonts, etc)

No pagination - display all sites and subnets.

13. Is accessibility an issue? Do we need 5.08 compliance?

None

14. Review the types and lengths of fields in the tables in the docs

15. Is the ipAddress data type appropriate for the IP address in the subnets table?

16. What is the correct database data type of subnet mask bits?

17. What is the correct database data type of the VLAN number?

18. What type of data is printers.print server?

19. How many users will we have, in any capacity? (Admins, read-only users, etc)

Primary admins - max 6

Readonly users - max 50

No self-registration (admins will create these accounts)

Okay for users to reset their own passwords

Admins need to be able to create, update, delete any accounts in the system (including reset passwords)

Most of the activity in the system comes from equipment - adding, moving, etc.

Subnets are next. Sites do not change often at all.













