# Podcast Outreach Automation System

This system automates podcast guest outreach using:
- Manus (decision engine)
- Notion (database / CRM)
- Gmail (email sending + reply detection)

## Overview

This is a state-based outreach system.

Each podcast moves through the following statuses:

Not Started → Intro Msg Sent → 1st Followup → 2nd Followup → 3rd Followup → Responded → Scheduling → Scheduled

Manus checks the database, decides what to do next, sends emails, and updates the system.

## Key Features

- Automated intro + follow-ups
- AI-powered personalization
- Smart contact addressing (host name vs team)
- Controlled escalation (timed follow-ups)
- Manual takeover when conversation starts

## Stack

- Notion → source of truth
- Manus → logic + execution
- Gmail → sending + reply tracking

## How It Works

1. Leads are added to Notion and marked "Not Started"
2. Manus runs on a schedule
3. Manus:
   - Generates personalization
   - Sends emails
   - Updates status
4. Replies are manually labeled in Gmail
5. Manus detects replies → stops automation

## Philosophy

This is not just outreach automation.

This is a repeatable distribution system that can be cloned for:
- clients
- partnerships
- investor outreach
