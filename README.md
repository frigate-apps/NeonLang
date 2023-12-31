<picture>
  <source media="(prefers-color-scheme: dark)" srcset="NeonLang-logo.svg">
  <img src="NeonLang-logo.svg" alt="NeonLang-Logo" height="128">
</picture>

# NeonBuild 1.0

NeonBuild 是一种代码生成器，提前尝试改进语法


```cpp

char %name% (%Param%) { %Code% }
float %name% (%Param%) { %Code% }
int %name% (%Param%) { %Code% }
void %name% (%Param%) { %Code% }
int %Param%;

#:"代码文件名字" Api
[int:h=10, w=20, slr=60]






void Hello [int:h, w, slr] [float:maot, w2, sl3r]
		编译
	↓ ↓	↓	↓
int h = 10, w=20, slr = 60;
void Hello (int h, int w, int slr, float maot, float w2, float slr3) {
}
```

配置文件格式: yaml、json、ini、TOML、
你们要投票要哪个配置文件格式?


| 系统 | 名字 | 支持 | 
|:--:|:--:|:--:|
| Wnodws | NSON、TOML  | ✅ |
| Wnodws | NeonLang | ✅ |
| NoteOS | NeonLang | ✅ |
| Mac | NeonLang | ✅ |

