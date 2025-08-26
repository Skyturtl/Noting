<%*
let title = tp.file.title;
let tags;
const fileName = tp.file.folder();
if (true) {
	title = "HW"
    tags = fileName.replaceAll(" ", "_");
    tp.file.rename("HW for " + fileName);
}


tR += `---
title: ${title}
created: ${tp.file.creation_date("Do MMMM YYYY")}
last modified: ${tp.file.last_modified_date("Do MMMM YYYY")}
Tags: [${tags}, HW]
---
`;
%>