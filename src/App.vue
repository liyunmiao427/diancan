<template>
  <div class="app">
    <div class="content-wrapper">
      <!-- 顶部：小朱点餐 -->
      <header class="header">
        <h1>小朱点餐</h1>
      </header>

      <!-- 菜品网格 -->
      <main class="dishes-grid">
        <!-- 西红柿炒鸡蛋 -->
        <div class="dish-card">
          <h2 class="dish-title">西红柿炒鸡蛋</h2>
          
          <!-- 图片 -->
          <div class="image-container">
            <img 
              src="/dish1.jpeg" 
              alt="西红柿炒鸡蛋"
              class="dish-image"
              @error="handleImageError"
            />
          </div>

          <!-- 做法教程 -->
          <div class="recipe-section">
            <div class="ingredients">
              <h4>食材：</h4>
              <p>西红柿、鸡蛋、葱花、盐、糖</p>
            </div>

            <div class="steps">
              <h4>步骤：</h4>
              <ol>
                <li>西红柿切块，鸡蛋打散</li>
                <li>先炒鸡蛋盛起，再炒西红柿</li>
                <li>混合翻炒，调味即可</li>
              </ol>
            </div>
          </div>
        </div>

        <!-- 葱花煎蛋 -->
        <div class="dish-card">
          <h2 class="dish-title">葱花煎蛋</h2>
          
          <!-- 图片 -->
          <div class="image-container">
            <img 
              src="/dish2.jpeg" 
              alt="葱花煎蛋"
              class="dish-image"
              @error="handleImageError"
            />
          </div>

          <!-- 做法教程 -->
          <div class="recipe-section">
            <div class="ingredients">
              <h4>食材：</h4>
              <p>鸡蛋 4 个，香葱 1 小把，盐少许，食用油 2 勺</p>
            </div>

            <div class="steps">
              <h4>步骤：</h4>
              <ol>
                <li>香葱切细葱花；鸡蛋打入碗中，加葱花、盐，充分搅打均匀</li>
                <li>平底锅烧热，倒少许油，油热后倒入蛋液，转中小火</li>
                <li>底部凝固后，用铲子翻一面，两面煎至金黄，关火盛出</li>
              </ol>
            </div>
          </div>
        </div>

        <!-- 凉拌黄瓜 -->
        <div class="dish-card">
          <h2 class="dish-title">凉拌黄瓜</h2>
          
          <!-- 图片 -->
          <div class="image-container">
            <img 
              src="/dish3.jpeg" 
              alt="凉拌黄瓜"
              class="dish-image"
              @error="handleImageError"
            />
          </div>

          <!-- 做法教程 -->
          <div class="recipe-section">
            <div class="ingredients">
              <h4>食材：</h4>
              <p>黄瓜 2 根，蒜末 3 瓣，小米辣 1 个（可选），生抽 2 勺，香醋 1 勺，白糖少许，香油、盐适量</p>
            </div>

            <div class="steps">
              <h4>步骤：</h4>
              <ol>
                <li>黄瓜洗净拍裂，切成段，放入碗中，加少许盐腌制 10 分钟</li>
                <li>小碗调酱汁：蒜末 + 小米辣 + 生抽 + 香醋 + 白糖 + 香油，搅拌均匀</li>
                <li>黄瓜腌出水分后倒掉，倒入调好的酱汁，拌匀即可</li>
              </ol>
            </div>
          </div>
        </div>

        <!-- 清炒土豆丝 -->
        <div class="dish-card">
          <h2 class="dish-title">清炒土豆丝</h2>
          
          <!-- 图片 -->
          <div class="image-container">
            <img 
              src="/dish4.jpeg" 
              alt="清炒土豆丝"
              class="dish-image"
              @error="handleImageError"
            />
          </div>

          <!-- 做法教程 -->
          <div class="recipe-section">
            <div class="ingredients">
              <h4>食材：</h4>
              <p>土豆 1 个，青椒半根（可选），蒜末 2 瓣，盐、白醋、食用油适量</p>
            </div>

            <div class="steps">
              <h4>步骤：</h4>
              <ol>
                <li>土豆去皮，切成均匀细丝，放入清水中浸泡 5 分钟，洗掉淀粉</li>
                <li>青椒切丝，蒜末备好</li>
                <li>热锅倒油，放入蒜末爆香，加入土豆丝、青椒丝，大火快速翻炒</li>
                <li>快熟时加少许白醋提脆，最后加盐调味，翻炒均匀出锅</li>
              </ol>
            </div>
          </div>
        </div>

        <!-- 蒜香油麦菜 -->
        <div class="dish-card">
          <h2 class="dish-title">蒜香油麦菜</h2>
          
          <!-- 图片 -->
          <div class="image-container">
            <img 
              src="/dish5.jpeg" 
              alt="蒜香油麦菜"
              class="dish-image"
              @error="handleImageError"
            />
          </div>

          <!-- 做法教程 -->
          <div class="recipe-section">
            <div class="ingredients">
              <h4>食材：</h4>
              <p>油麦菜 1 把，蒜末 4 瓣，盐、蚝油、食用油适量</p>
            </div>

            <div class="steps">
              <h4>步骤：</h4>
              <ol>
                <li>油麦菜洗净，切成两段</li>
                <li>热锅倒油，放入蒜末炒出香味</li>
                <li>放入油麦菜，大火快速翻炒至菜叶变软</li>
                <li>加少许蚝油、盐调味，翻炒均匀立即出锅</li>
              </ol>
            </div>
          </div>
        </div>

        <!-- 可乐鸡翅 -->
        <div class="dish-card">
          <h2 class="dish-title">可乐鸡翅（小白本命肉菜）</h2>
          
          <!-- 图片 -->
          <div class="image-container">
            <img 
              src="/dish6.jpeg" 
              alt="可乐鸡翅"
              class="dish-image"
              @error="handleImageError"
            />
          </div>

          <!-- 做法教程 -->
          <div class="recipe-section">
            <div class="ingredients">
              <h4>食材：</h4>
              <p>鸡翅中 8 个、可乐 330ml、姜片 3 片、料酒 1 勺、生抽 2 勺、老抽半勺、白芝麻少许（点缀）</p>
            </div>

            <div class="steps">
              <h4>步骤：</h4>
              <ol>
                <li>鸡翅背面划 2 刀方便入味；冷水下锅，加姜片 + 料酒，大火煮出浮沫，捞出用温水冲净，彻底控干水分（防煎油溅）</li>
                <li>平底锅放少许油，中小火，鸡翅皮朝下，煎至两面金黄微焦</li>
                <li>加生抽 + 老抽，快速翻炒上色；倒入可乐，没过鸡翅，大火烧开后撇净浮沫，转中小火焖 15 分钟</li>
                <li>开大火收汁，期间不停轻轻翻动防止粘锅，直到汤汁浓稠裹住鸡翅，撒白芝麻出锅</li>
              </ol>
            </div>
          </div>
        </div>

        <!-- 青椒炒肉 -->
        <div class="dish-card">
          <h2 class="dish-title">青椒炒肉（下饭王者）</h2>
          
          <!-- 图片 -->
          <div class="image-container">
            <img 
              src="/dish7.jpeg" 
              alt="青椒炒肉"
              class="dish-image"
              @error="handleImageError"
            />
          </div>

          <!-- 做法教程 -->
          <div class="recipe-section">
            <div class="ingredients">
              <h4>食材：</h4>
              <p>猪前腿 / 里脊 180g、青椒 2 个、蒜末 2 瓣、姜片 2 片、料酒 1 勺、生抽 1.5 勺、盐少许、食用油适量</p>
            </div>

            <div class="steps">
              <h4>步骤：</h4>
              <ol>
                <li>猪肉切薄片 / 细丝，加料酒 + 半勺生抽，抓匀腌制 10 分钟去腥；青椒去籽去筋，切成斜段</li>
                <li>热锅，不放油先下肉片，中小火煸炒至出油、表面微黄，盛出备用</li>
                <li>锅中留底油，下姜蒜爆香，转大火倒入青椒，炒至青椒起虎皮、微微变软</li>
                <li>倒回炒好的肉片，加剩余生抽 + 少许盐，大火快速翻炒 1 分钟，出锅</li>
              </ol>
            </div>
          </div>
        </div>

        <!-- 蒜蓉鸡胸肉 -->
        <div class="dish-card">
          <h2 class="dish-title">蒜蓉鸡胸肉（低脂不柴）</h2>
          
          <!-- 图片 -->
          <div class="image-container">
            <img 
              src="/dish8.jpeg" 
              alt="蒜蓉鸡胸肉"
              class="dish-image"
              @error="handleImageError"
            />
          </div>

          <!-- 做法教程 -->
          <div class="recipe-section">
            <div class="ingredients">
              <h4>食材：</h4>
              <p>鸡胸肉 1 块（约 200g）、蒜末 5 瓣、生抽 1 勺、蚝油 1 勺、盐少许、白胡椒粉少许、食用油 1.5 勺</p>
            </div>

            <div class="steps">
              <h4>步骤：</h4>
              <ol>
                <li>鸡胸肉横片成 2 片（变薄易熟不柴），切条；加少许盐 + 白胡椒粉 + 半勺生抽，抓匀腌 10 分钟</li>
                <li>热锅放少许油，下蒜末，小火炒至微微金黄出蒜香（别糊！）</li>
                <li>转中火，倒入鸡胸肉条，快速滑散，炒至肉条全部变白、无一丝粉色</li>
                <li>加蚝油，翻炒 10 秒入味，关火出锅</li>
              </ol>
            </div>
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<script setup>
const handleImageError = (e) => {
  // 如果图片加载失败，使用备用图片或隐藏
  e.target.style.display = 'none';
}
</script>

<style scoped>
.app {
  width: 100%;
  height: 100%;
  min-height: 100vh;
  --color1: rgb(108, 231, 221);
  --color2: rgb(250, 255, 178);
  background-color: var(--color1);
  background-image: linear-gradient(45deg, var(--color2) 25%, transparent 25%, transparent 75%, var(--color2) 75%, var(--color2)), 
                    linear-gradient(45deg, var(--color2) 25%, var(--color1) 25%, var(--color1) 75%, var(--color2) 75%, var(--color2));
  background-size: 60px 60px;
  background-position: 0 0, 30px 30px;
  padding: 20px;
  box-sizing: border-box;
}

.content-wrapper {
  max-width: 1400px;
  margin: 0 auto;
}

.header {
  text-align: center;
  margin-bottom: 30px;
}

.header h1 {
  font-size: 2.5rem;
  color: #333;
  font-weight: 700;
  margin: 0;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
}

.dishes-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
  padding: 0 10px;
}

.dish-card {
  background: rgba(255, 255, 255, 0.95);
  border-radius: 15px;
  padding: 15px;
  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.15);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.dish-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
}

.dish-title {
  font-size: 1.3rem;
  color: #d32f2f;
  text-align: center;
  margin-bottom: 12px;
  font-weight: 700;
}

.image-container {
  width: 100%;
  height: 180px;
  margin-bottom: 15px;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
}

.dish-image {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
}

.recipe-section {
  color: #333;
  font-size: 0.9rem;
}

.ingredients,
.steps {
  margin-bottom: 12px;
}

.ingredients h4,
.steps h4 {
  font-size: 1rem;
  color: #555;
  margin-bottom: 6px;
  font-weight: 600;
}

.ingredients p {
  color: #666;
  font-size: 0.85rem;
  line-height: 1.5;
  margin: 0;
}

.steps ol {
  padding-left: 20px;
  line-height: 1.6;
  margin: 0;
}

.steps li {
  margin-bottom: 4px;
  color: #666;
  font-size: 0.85rem;
}

@media (max-width: 1024px) {
  .dishes-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 768px) {
  .header h1 {
    font-size: 2rem;
  }
  
  .dishes-grid {
    grid-template-columns: 1fr;
    gap: 15px;
  }
  
  .dish-title {
    font-size: 1.2rem;
  }
  
  .image-container {
    height: 200px;
  }
}
</style>

