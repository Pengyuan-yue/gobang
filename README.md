# 五子棋游戏 (Gobang)

这是一个基于网页的五子棋游戏，支持本地双人对战、人机对战和在线对战功能。

## 功能特点

- **三种游戏模式**:
  - 本地双人对战
  - 人机对战（三个难度级别）
  - 在线对战（创建房间或加入房间）
- **核心功能**:
  - 15×15标准棋盘
  - 悔棋功能
  - 重新开始游戏
  - 胜负判定
- **AI算法**:
  - 简单：随机落子
  - 中等：启发式评估
  - 困难：Minimax算法+Alpha-Beta剪枝

## 技术栈

- **前端**: React + Canvas
- **后端**: Node.js + Express + WebSocket
- **AI算法**: JavaScript实现

## 安装与运行

### 前提条件
- Node.js (v14+)
- npm (v6+)

### 步骤

1. 克隆仓库:
   ```bash
   git clone https://github.com/yourusername/gobang.git
   cd gobang
   ```

2. 安装依赖:
   ```bash
   cd client
   npm install
   cd ../server
   npm install
   ```

3. 启动服务器:
   ```bash
   cd server
   npm start
   ```

4. 启动客户端:
   ```bash
   cd client
   npm start
   ```

5. 打开浏览器访问: `http://localhost:3000`

## 项目结构

```
gobang/
├── client/             # 前端代码
│   ├── public/
│   ├── src/
│   │   ├── ai/         # AI算法实现
│   │   ├── components/ # React组件
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
├── server/             # 后端代码
│   ├── index.js        # 服务器入口
│   └── package.json
└── README.md
```

## 在线对战说明

1. 创建房间：点击"创建房间"按钮，系统会生成房间ID
2. 加入房间：在输入框中输入房间ID，点击"加入房间"
3. 游戏开始：双方玩家加入后自动开始游戏
4. 黑棋先行，轮流落子

## 未来改进

- 添加音效
- 实现计时器功能
- 优化AI算法
- 添加更多棋盘主题