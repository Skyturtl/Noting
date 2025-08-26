<%*
let title = tp.file.title;
let tags;
if (title.startsWith("Untitled")) {
	title = tp.file.folder()
    tags = title
    tp.file.rename(title + " " + tp.date.now("Do MMMM YYYY"));
}


tR += `---
title: ${title}
created: ${tp.file.creation_date("Do MMMM YYYY")}
last modified: ${tp.file.last_modified_date("Do MMMM YYYY")}
Tags: [${tags}, HW]
---
`;
%>