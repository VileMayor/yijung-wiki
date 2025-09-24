<%* setTimeout(() => { // Get the path to the new file 
const newFile = tp.file.find_tfile(tp.file.path(true)) // Process the frontmatter 
app.fileManager.processFrontMatter(newFile, (frontmatter) => { // Add a new field 
frontmatter.title = tp.file.title
frontmatter.draft = false
// Or delete the properties you don't want 
 }) }, 300) %><%*
// Get the active file using the Templater API.
const file = tp.file.find_tfile(tp.file.path(true));

// Prompt for the new title.
const newTitle = await tp.system.prompt("Enter new title:");

// Process the frontmatter to update the properties.
if (newTitle) {
    await app.fileManager.processFrontMatter(file, (frontmatter) => {
        frontmatter.title = newTitle;
        frontmatter.draft = false; // Example: Set draft to false
    });
    // Rename the file to match the new title if desired.
    // Make sure the title is safe for file names.
    await tp.file.rename(newTitle);
}

// Ensure the function returns nothing to avoid unwanted text insertion.
_%>
