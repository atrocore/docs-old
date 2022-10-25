# Documentation Writing Standards

## Using special characters

- Mention Breadcrumbs in backquotes, eg `Dashboard / Brands`.
- Define actions and button names, eg `Action name`.
- For entity names, panel names, field names and all other system-specific names – first letter of each word should be capitalized, eg Product Category, but Product data record. 
- Use double quotes only in exceptional cases, where other cases from these standards cannot be applied.
- Single quote can be used only as apostrophe, do not use it in other cases.
- Use "–", not "-", if you need a "dash" character, eg "Field Name – description of the field name". 
- Avoid using other special characters.

## Using references
- Do not describe same functionality on different places, choose the most appropriate place and describe this functionality there.
- On all other places reference to that chapter by using relative links with heading anchors, not absolute links, eg
```
[Correcting errors by clearing system cache](../../atrocore/admin-guide/correcting-errors.md#clearing-system-cache)
```
- If the files are moved to other places of documentation structure is changed, check if references are still working.

## Using double quotes

- To indicate words used ironically, with reservations, or in some unusual way, eg "right" choice.
- To set off words used as words, terms, options etc, eg the term "Entity", "dash" character, select option "Relationship".
- For module names, eg the module "Advanced data types".
- To state options in select lists, eg please choose "Relationship" as a type.

## Internal comments
- Internal comments can be used as reminder, for review comments about what should be improved, stating "To Dos" etc.
- Use HTML comment markup for it, because it is not visible to the readers, eg 
```
<!-- To Do 20.10.22
1. add reference to xxxx
2. add description about yyy
-->
```

## File naming

- Use speaking file names, eg filter-apply-and-reset-buttons.jpg, NOT filter4.jpg.
- Use only small letters in file names, eg filder.jpg, not Filter.jpg.
- Do not use spaces, exchange spaces with "-" to separate works, eg reset-button.jpg.
- Usually do not use underscore "\_" in the file names. Use it only in excentional cases to explicitly emphasize something in the file name, eg reset-button_2022.jpg.
- Do not use special characters and specific language letters, like ä,ü,ß,ö and other.
- Use file names without extensions as labels for your images (which are in brackets), eg \[attribute-tab-create\]\(../\_assets/user-guide/attribute_tab/attribute-tab-create.png\).

## General recommendations

- Do not write words which can be deleted without losing the sense for the sentence.
- Do not write sentences which can be deleted in full without losing the sense for the sentence.
- Do not describe what is already so obvious, like "see the picture bellow".
- Do not start a note with "Please note" or with something similar.
- Do not use fully capitalized words, eg "PANEL".
- Use bold font to highlight important information, eg "**Channel** – is a destination for product information".
- Use italic font only to highlight something in a different matter if bold font is already used.
- Use relative hyperlinks.
- Do not use absolute hyperlinks.
- Use of HTML is allowed only in exceptional cased.
- Use multi-level headings.
- Use tables to highlight plain information structures.
- Use bullet points for lists.
- Avoid using bullet points for multi-line sentences.

## Using git branches for writing documentation
- To describe a new or improve an existing topic always create a new branch from master branch (in VSCode option "create branch from..").
- If documentation is written for a certain issue, use the prefix "i-" and issue id as a branch name, eg "i-5ff5e2e73148ba911"-
- A branch may be created for multiple issues, in this case mention all addressed issues, eg "i-5ff5e2e73148ba911-5ff5e2e73148ba912-5ff5e2e73148ba913".
- A branch may be related to a whole milestone, in this case use the prefix "m-" and milestone id as a branch name, eg "m-5ff5e2e73148ba911".
- A branch may be created proactively, without having an issue for it, in this case, use some "speaking" name, eg "improving-inheritance-description".
- Optionally, some "speaking" comment may be added, eg "i-5ff5e2e73148ba911-added-SKU-field-to-a-product".
- After all changed are committed to branch create a pull request.
- After the pull request is merged the remote branch will be removed by the reviewer. A local branch should be deleted by the submitter.

In other topics follow the recommendations of this Guide: https://developers.google.com/style
