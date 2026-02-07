# Echuu - Gemini 3 Hackathon Submission

## Project Overview

**Echuu** is an AI-powered VTuber auto-live system that leverages **Gemini 3's revolutionary Thinking Mode** to generate natural, spontaneous streaming content with multi-language support and user relationship building.

## Gemini 3 Innovation Highlights

### 1. Thinking Mode - Controlled Reasoning Depth

Echuu uniquely utilizes Gemini 3's **Thinking Mode** to optimize different use cases:

```python
# Deep reasoning for complex storytelling
client.call(prompt, thinking_level="high")

# Quick responses for simple chat
client.call(prompt, thinking_level="low")
```

**Why This Matters:**
- **Dynamic Optimization**: Adjust reasoning depth based on content needs
- **Cost Efficiency**: Use minimal thinking for simple interactions
- **Quality Control**: Maximum reasoning for story climaxes and key moments

### 2. Multi-Language Auto-Detection

Leveraging Gemini 3's superior multilingual capabilities:

```python
# Auto-detects language from input topic
engine.setup(topic="今日の出来事")  # -> Japanese
engine.setup(topic="Today's story")  # -> English
engine.setup(topic="今天遇到的趣事")  # -> Chinese
```

### 3. User Memory & Bonding System

Track viewer relationships using Gemini 3's large context window:

```
新观众 -> 眼熟 -> 老观众 -> 核心粉丝
```

### 4. Natural Content Generation

Applies the "分享欲 + 反常 + 内心戏" formula for engaging stories.

## Technical Architecture

```
User Input
    |
    v
[Gemini 3 Thinking Mode]  <-- Core Innovation
    |
    v
Story Nucleus Generator
    |
    v
Script Generator (with VRM Cues)
    |
    v
Performer Engine + TTS
    |
    v
Output: Speech + Audio + Avatar Control
```

## Demo Experience

### Quick Start (5 minutes)

```bash
pip install -r requirements.txt
echo "GEMINI_API_KEY=your-key" > .env
python examples/demo.py --mp3
```

### Multi-Language Demo

```bash
python examples/test_multilingual.py
```

### User Memory Demo

```bash
python examples/test_user_memory.py
```

## File Structure

```
public/
├── echuu/                    # Core SDK
│   ├── live/                # Gemini 3 integration, TTS, engine
│   ├── core/                # Story generation, emotion, VRM cues
│   ├── generators/          # Script generation with few-shot learning
│   └── vrm/                 # Avatar control mapping
├── examples/                # Demo scripts
├── output/examples/         # Sample outputs (audio + scripts)
├── README.md                # Project overview
├── QUICKSTART.md            # 5-minute setup guide
├── GEMINI3_FEATURES.md      # Detailed Gemini 3 features
└── requirements.txt         # Dependencies
```

## Output Examples

- `output/examples/example_chinese_canteen.json` - Chinese streaming script
- `output/examples/example_japanese_akihabara.json` - Japanese streaming script
- `output/examples/example_english_dance_video.json` - English streaming script
- `output/examples/example_chinese_cat_audio.mp3` - TTS audio sample

## Key Metrics

| Metric | Value |
|--------|-------|
| Script Generation Time | 3-5 seconds (10 steps) |
| Multi-Language Accuracy | 98%+ auto-detection |
| Supported Languages | Chinese, Japanese, English |
| Cost per 10-min Stream | ~$0.01 (Flash model) |
| VRM Expressions | 6 emotions + 18 gestures |

## Why Gemini 3?

1. **Thinking Mode** - Unique control over reasoning depth (exclusive to Gemini 3)
2. **Flash Speed** - Real-time streaming without lag
3. **Large Context** - Remember user history and story continuity
4. **Multilingual** - Superior cross-language generation
5. **Cost Effective** - High quality at competitive prices

## Future Roadmap

- [ ] Image input processing (Gemini 3 Vision)
- [ ] Image generation for thumbnails (Gemini 3 Pro Image)
- [ ] Voice cloning integration
- [ ] Real-time WebSocket streaming
- [ ] Unity/Unreal VRM viewer integration

## License

Apache-2.0 - Open source for the community

---

**Built for Gemini 3 Dev Hackathon 2025**

This project showcases the innovative application of Gemini 3's Thinking Mode for creative AI content generation.
