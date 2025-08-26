<%*
let title = tp.file.title;
let tags;
if (true) {
	title = tp.file.folder();
    tags = title.replaceAll(" ", "_");
    tp.file.rename("HW for " + title);
}


tR += `---
title: ${title}
created: ${tp.file.creation_date("Do MMMM YYYY")}
last modified: ${tp.file.last_modified_date("Do MMMM YYYY")}
Tags: [${tags}, HW]
---
`;
%>