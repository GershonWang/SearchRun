<template>
  <h1>按钮主界面</h1>
  <input type="file" id="file-input">
</template>
<script setup lang="ts">
// import * as fs from 'fs';
// import * as path from 'path';

// function getFilesInDir(dir: string) {
//   const files = fs.readdirSync(dir);
//   const result: any[] = [];

//   files.forEach((file: any) => {
//     const filePath = path.join(dir, file);
//     const stat = fs.statSync(filePath);

//     if (stat.isDirectory()) {
//       result.push(...getFilesInDir(filePath));
//     } else {
//       result.push(filePath);
//     }
//   });

//   return result;
// }

// const files = getFilesInDir('/path/to/directory');
// console.log(files);

// const filePath = 'C:\Users\Administrator\Desktop\key.txt';
// const fileName = path.basename(filePath); // 获取文件名，返回 'file.txt'
// console.log('fileName', fileName);
// const dirName = path.dirname(filePath); // 获取文件所在目录，返回 '/path/to'
// console.log('dirName', dirName);
// const extName = path.extname(filePath); // 获取文件扩展名，返回 '.txt'
// console.log('extName', extName);
// const absolutePath = path.resolve(filePath); // 获取文件的绝对路径
// console.log('absolutePath', absolutePath);

const fileInput = document.getElementById('file-input');
if (fileInput != null) {
  fileInput.addEventListener('change', (event) => {
    console.log('event',event);
    // if (event != null && event.target != null) {
    //   const file = event.target.files[0];
    //   const reader = new FileReader();
    //   reader.onload = (event) => {
    //     if (event != null && event.target != null) {
    //       const fileContent = event.target.result;
    //       console.log(fileContent);
    //     }
    //   };
    //   reader.readAsText(file);
    // }
  });
}
</script>

<style scoped></style>