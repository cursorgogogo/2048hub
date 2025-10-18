# 2048 Hub - 2048游戏集合站点

一个专业的2048游戏集合站点，为用户提供便捷的游戏选择和游玩体验。

## 功能特点

- 🎮 **多游戏集合**: 集成多种2048游戏变种
- 📱 **响应式设计**: 支持手机、平板、电脑等各种设备
- ⚡ **即点即玩**: 无需下载，直接在浏览器中游玩
- 🔄 **无感知切换**: 使用iframe技术，无需跳转页面
- 🎯 **SEO优化**: 完整的SEO优化，提升搜索引擎排名
- 🛠️ **易于扩展**: 简单的配置即可添加新游戏

## 技术栈

- HTML5
- CSS3 (Flexbox + Grid)
- Vanilla JavaScript
- 响应式设计

## 文件结构

```
2048hub/
├── index.html          # 主页面
├── styles.css          # 样式文件
├── script.js           # JavaScript逻辑
├── games-config.json   # 游戏配置文件
├── sitemap.xml         # 网站地图
├── robots.txt          # 搜索引擎爬虫配置
└── README.md           # 说明文档
```

## 添加新游戏

### 方法1: 修改配置文件

编辑 `games-config.json` 文件，在 `games` 数组中添加新游戏：

```json
{
  "id": "new-game",
  "title": "新游戏名称",
  "description": "游戏描述",
  "icon": "🎮",
  "url": "https://new-game.com",
  "iframe": true,
  "category": "new-category",
  "difficulty": "medium",
  "tags": ["标签1", "标签2"]
}
```

### 方法2: 使用JavaScript API

```javascript
// 添加新游戏
GameHub.addGame({
  id: 'new-game',
  title: '新游戏名称',
  description: '游戏描述',
  icon: '🎮',
  url: 'https://new-game.com',
  iframe: true
});

// 移除游戏
GameHub.removeGame('game-id');

// 获取所有游戏
const allGames = GameHub.getAllGames();

// 选择特定游戏
GameHub.selectGame('game-id');
```

## SEO优化

- 完整的meta标签配置
- Open Graph和Twitter Card支持
- 结构化数据标记
- 网站地图(sitemap.xml)
- 搜索引擎爬虫配置(robots.txt)
- 语义化HTML结构

## 部署说明

1. 将所有文件上传到Web服务器
2. 确保服务器支持HTTPS（推荐）
3. 配置域名解析到服务器
4. 更新 `games-config.json` 中的游戏URL为实际地址
5. 根据需要调整SEO元数据

## 浏览器支持

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 许可证

MIT License
