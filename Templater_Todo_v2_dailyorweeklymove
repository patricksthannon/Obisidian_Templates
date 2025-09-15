<%*
const dailyFolder = "/Daily_Notes/";
const weeklyFolder = "/Weekly_Notes/";
const filename = tp.file.title;

// Check if it's a daily note: YYYY-MM-DD
if (/^\d{4}-\d{2}-\d{2}$/.test(filename)) {
    const newPath = `${dailyFolder}${filename}`;
    if (tp.file.path !== newPath) {
        await tp.file.move(newPath);
    }
}
// Check if it's a weekly note: YYYY - W## (handles 1–2 digit weeks)
else if (/^\d{4}\s-\sW\d{1,2}$/.test(filename)) {
    const newPath = `${weeklyFolder}${filename}`;
    if (tp.file.path !== newPath) {
        await tp.file.move(newPath);
    }
}
%>
