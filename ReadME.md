# Wrap Discord Bot – Command Reference

Welcome to **Wrap** by Harshit! Below you'll find all available commands, usage examples, and permission requirements for managing your server with Wrap.

---

## 🎯 Available Slash Commands

### 1. `/setup-wrap`
- **Description:** Configure the Wrap bot for this server (posts to designated channel)
- **Permission Required:** Administrator
- **Options:**
  - `threshold` (optional): Reaction threshold for viral messages (default: 10)
- **Example:**
  ```
  /setup-wrap threshold:15
  ```

### 2. `/log-event`
- **Description:** Manually log a server event
- **Permission Required:** Manage Messages
- **Options:**
  - `event` (required): Event description
  - `priority` (optional): Event priority (Low/Medium/High)
- **Example:**
  ```
  /log-event event:"Server hit 1000 members!" priority:High
  ```

### 3. `/generate-wrap`
- **Description:** Generate and post a server wrap
- **Permission Required:** Administrator
- **Example:**
  ```
  /generate-wrap
  ```

### 4. `/server-stats`
- **Description:** View server event statistics
- **Permission Required:** Everyone
- **Options:**
  - `show_details` (optional): Show recent logs with IDs for removal
- **Examples:**
  ```
  /server-stats
  /server-stats show_details:true
  ```

### 5. `/remove-log`
- **Description:** Remove a specific log entry by ID
- **Permission Required:** Administrator
- **Options:**
  - `log_id` (required): The ID of the log entry to remove
- **Example:**
  ```
  /remove-log log_id:123
  ```

---

## 🤖 Automatic Event Tracking

The bot automatically tracks these events:
- 🔥 **Viral Messages:** When messages get reactions above threshold
- 👥 **Member Joins:** New members joining the server
- 👋 **Member Leaves:** Members leaving the server
- 🚫 **Member Bans:** When members get banned
- 🆕 **Channel Creation:** New channels being created

---

## 📋 Command Usage Examples

```bash
# Initial setup (Admin only)
/setup-wrap threshold:10

# Log custom events (Moderators)
/log-event event:"Epic meme war started" priority:High
/log-event event:"Bot updates completed"

# View statistics
/server-stats
/server-stats show_details:true

# Generate wrap story (Admin only)
/generate-wrap

# Remove unwanted logs (Admin only)
/remove-log log_id:15
```

---

## 🔐 Permission Requirements

| Command         | Required Permission |
|-----------------|--------------------|
| /setup-wrap     | Administrator      |
| /log-event      | Manage Messages    |
| /generate-wrap  | Administrator      |
| /server-stats   | None (Everyone)    |
| /remove-log     | Administrator      |

---

The bot is currently **online and ready to use!**