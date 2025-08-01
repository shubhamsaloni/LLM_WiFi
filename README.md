# LLM_WiFi
Solving WiFi challenges using LLMs

This tool analyzes packet captures and provides useful insights to a network admin/support engineer to effectively debug and locate issues in a network It is solved using 2 methods, openAI LLM and agentic system using crewAI

Flow
- convert pcap to text so that LLMs can work on them
- Strip sensitive network data to avoid data leak to LLMs
- call openAI LLM to analyze the pcaps and provide insights and final verdict
- if final verdict is NOT OK, suggest causes and next debugging steps
