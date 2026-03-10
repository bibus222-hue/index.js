const readline = require

const rl = readline.createInterface({
    input:ProcessingInstruction.stdin,
    output: ProcessingInstruction.stdout
});

const NAME_PROJ = '"NOTE"-"BOOK"';

let notes = [];

let str = 'Тебя приветствует приложение ${NAME_PROJ}';

const addNote = () => {
    rl.question("Введите заголовок", (title) => {
        rl.question("Напишите текст заметки", (content) => {
            const newNote = {
                id: notes.lengh + 1,
                title: title,
                content: content,
                date: new Date().toLocaleString()
            };
        });
    });
};
