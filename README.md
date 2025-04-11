# Git_Course_lap_2

## How to remove branch locally and remotly?
 #### step 1 :
-  ` go to parent branch ` 
#### step 2 :
*   ##### 1- To romve branch locally
    * ` git branch -d branch_name (this can be used when all changes of current branch are merged to parent branch ).`
    *  ` git branch -D branch_name (this enforce the branch to be deleted despite of the changes are merged or not ).`
  ##### 2- To remove branch remotly
   - ` git push origin --delete branch_name`

## Annotated Tags & Lightweight Tags 
  #### Annotated Tags :
   * ` Stored as full objects in Git’s database.`
   * ` Contain extra metadata :`
      * `Tagger name & email`
      * `Date of tagging`
   * `Createion way :`

      * `git tag -a v1.7 -m "Release version "`
 #### Lightweight Tags  :
  * ` Just a pointer to a specific commit.`
  * ` No extra metadata`
  * `Createion way :`

     * `git tag v1.7-lite` 
## When to use Rebase?
 * ` When to need to update featured-branch and rewrite the commits history to move featured-branch commits at the top of commits history.`
  * `Createion way :`

     * `git rebase -i HEAD~3  (Combines last 3 commits)`
 ## How to list tags in git?
 1. `List All Tags `
    * `git tag`
 2. `List Tags with Additional Details `
    
    * `git show-ref --tags`
 3. ` List Remote Tags `
    
    * `git ls-remote --tags origin`
 ## How to delete tags locally and remotly?
 1. #### ` Delete a Tag Locally `
    * ` Single Tag : `
       * ` git tag -d tag_name `
     
    * ` Delete Multiple Tags : `
       * ` git tag -d tag1 tag2 tag3 `
     
 2. #### ` Delete a Tag Remotly `
    
    * ` Single Tag : `    
       * ` git push origin --delete tag_name `
    * ` Delete Multiple Tags : `
      
       * ` git push origin --delete tag1 tag2 tag3 `   
         
