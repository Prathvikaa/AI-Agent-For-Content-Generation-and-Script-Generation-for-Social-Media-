# AI-Agent-For-Content-Generation-and-Script-Generation-for-Social-Media-
An AI content assistant that summarizes text, generates video/reel scripts, and suggests trending content ideas. Built with LangChain Groq (LLaMA3) and LangGraph for context-aware conversations, it helps creators quickly produce engaging scripts with minimal effort.

**Features**
1) Text Summarization
    -> Paste any text and get a concise AI-generated summary
    -> Handles different input formats (summarize: text, quotes, etc.)
2) Video/Reel Script Generation
    -> Creates short-form video scripts with hooks, engaging flow & call-to-actions
    -> Supports TikTok, Instagram Reels, YouTube Shorts
3) Trend-based Script Suggestions
    -> Generates trending content topics based on a chosen niche
    -> Includes hashtags, engagement tips & structure
4) Interactive Chat
    -> Works like a chatbot with memory of previous messages
    -> Fallback to normal conversation if no specific command is detected

**Tech Stack**

1) LLM API: LangChain Groq with LLaMA3-8B-8192
2) LangGraph: For state management & workflow
3) Pydantic: For structured message handling
4) Regex Patterns: To detect & process user commands
5) Python

**How It Works**

1) User enters a message, e.g.:
    -> summarize: your long text here
    -> create video script about AI tools in 2025
    -> trending script for fitness niche

2) Command detection → Regex identifies whether it’s a summary request, script request, or normal conversation.
   
3) LLM Execution
    -> For summaries → AI returns a short summary
    -> For scripts → AI generates a structured video script with hooks, sections & call-to-action
    -> For trend-based → AI suggests trending topics & scripts

4) The conversation history is tracked & remembered so AI can respond with context.
