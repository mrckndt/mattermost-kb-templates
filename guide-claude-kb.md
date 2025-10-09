# Creating a Custom KB Slash Command for Claude Code

This guide shows you how to create a custom slash command called `/kb` that transforms raw content into styled Knowledge Base articles using Claude Code's custom command feature.

## What are Claude Code Custom Slash Commands?

Custom slash commands in Claude Code allow you to create reusable prompts that can be invoked with a simple `/command-name` syntax. They're stored as Markdown files in your project's `.claude/commands/` directory and can accept arguments, making them perfect for repetitive tasks like formatting documentation.

## Overview

The `/kb` command will:

- Take unstructured content as input
- Analyze and structure it according to KB best practices
- Generate a fully styled HTML article with proper formatting
- Save the result as an HTML file for immediate use

## Setup Instructions

### 1. Create the Command Directory Structure

First, create the necessary directory structure for Claude Code custom commands:

```bash
mkdir -p ~/kbs/.claude/commands
cd ~/kbs/.claude/commands
```

### 2. Copy the KB Command File

Create the command file that will contain your prompt:

```bash
cp kb.md .claude/commands

```

## 3. Using the KB Command

### 1. Start Claude Code in Your Project Directory

Navigate to your KB project directory and start Claude Code:

```bash
cd ~/kbs
claude
```

### 2. Execute the KB Command

You can use the `/kb` command in two ways:

**Option A: Paste content directly**

```
/kb Your raw content here...
```

**Option B: Reference a file**

```
/kb @kb-article.txt
```

### 3. Review and Refine

The command will:

1. Analyze your content and provide insights
2. Generate a styled HTML file (e.g., `kb-article-heading.html`)
3. Save it in your current directory

After generation:

- Review the generated HTML file
- Make additional refinements by asking Claude to modify specific sections
- Publish when satisfied with the result

### 4. Exit when done

```bash
/exit
```

## Tips for Best Results

- **Prepare your content**: Organize your raw content with clear problem descriptions, solutions, and any error messages
- **Include context**: Mention the product version, audience, and any prerequisites
- **Iterate**: Use follow-up prompts to refine specific sections or styling
- **Preview**: Paste the generated HTML file in Zendesk to preview before publishing

## Troubleshooting

### Command Not Found

If you get a "command not found" error:

1. Ensure you're in the correct directory (`~/kbs`)
2. Verify the command file exists at `~/kbs/.claude/commands/kb.md`
3. Restart Claude Code to reload custom commands

### Template Issues

If the generated HTML doesn't look right:

- Check that the entire prompt was copied correctly into `kb.md`
- Ensure your input content includes clear problem/solution structure
- Use follow-up prompts to adjust specific sections

### File Not Generated

If no HTML file is created:

- Make sure you have write permissions in the directory
- Check that the command completed without errors
- Try running the command with simpler test content first
