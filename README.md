# job-referal-platform

# AI-Assisted Job Referral Platform

A full-stack Job Referral Platform that allows recruiters to create job postings and manage referrals, while candidates can browse available jobs, refer friends, and track referral status.

The application is built using **Java Spring Boot, Spring Security, JWT, MySQL, and React.js**.

---

## Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Features](#features)
- [User Roles](#user-roles)
- [Technology Stack](#technology-stack)
- [System Architecture](#system-architecture)
- [Project Structure](#project-structure)
- [Database Design](#database-design)
- [Authentication & Authorization](#authentication--authorization)
- [Application Workflow](#application-workflow)
- [Backend API](#backend-api)
- [Frontend](#frontend)
- [Demo Credentials](#demo-credentials)
- [Prerequisites](#prerequisites)
- [Database Setup](#database-setup)
- [Backend Setup](#backend-setup)
- [Frontend Setup](#frontend-setup)
- [Running the Application](#running-the-application)
- [Testing the Application](#testing-the-application)
- [Sample API Requests](#sample-api-requests)
- [Security](#security)
- [Validation and Error Handling](#validation-and-error-handling)
- [Seed Data](#seed-data)
- [Optional Enhancements](#optional-enhancements)
- [Design Decisions](#design-decisions)
- [Future Improvements](#future-improvements)
- [Screenshots](#screenshots)
- [Author](#author)

---

# Overview

The Job Referral Platform provides a simple end-to-end workflow for managing employee/friend referrals for job opportunities.

There are two types of users:

1. **Candidate**
2. **Recruiter**

Candidates can browse job postings and submit referrals for their friends.

Recruiters can create job postings and review referrals submitted for their jobs.

The application uses JWT-based authentication and role-based authorization to ensure that users can access only the functionality allowed for their role.

---

# Problem Statement

The goal is to build a minimal, end-to-end job referral web application that supports:

- Secure user registration and login
- JWT-based authentication
- Password hashing
- Candidate and Recruiter roles
- Recruiter job creation
- Candidate job browsing
- Friend referral submission
- Referral status tracking
- Recruiter referral management
- RESTful APIs
- Relational database storage
- React-based frontend
- Demo seed data

---

# Features

## Authentication

- User registration
- User login
- JWT authentication
- BCrypt password hashing
- Role-based authorization
- Stateless authentication

## Recruiter Features

Recruiters can:

- Login securely
- Create job postings
- View their own job postings
- View referrals submitted for their jobs
- View candidate information
- View referred friend's information
- View recommendation messages
- Update referral status

## Candidate Features

Candidates can:

- Login securely
- Browse available jobs
- View job title
- View job description
- View location
- View minimum qualifications
- View required skills
- Refer a friend
- View submitted referrals
- Track referral status

## Referral Features

Each referral contains:

- Friend name
- Friend email
- Recommendation
- Candidate who submitted the referral
- Job
- Submission date
- Referral status

Referral statuses:

```text
PENDING
REVIEWED
