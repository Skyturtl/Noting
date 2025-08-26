<%*
let title = tp.file.title;
let tags;
let today = tp.date.now("MM-DD-YYYY")
if (true) {
	title = tp.file.folder()
    tags = title.replaceAll(" ", "_");
    tp.file.rename(today);
}

tR += `---
title: ${today}
created: ${tp.file.creation_date("Do MMMM YYYY")}
last modified: ${tp.file.last_modified_date("Do MMMM YYYY")}
Tags: [${tags}, Lecture]
---
`;
%>