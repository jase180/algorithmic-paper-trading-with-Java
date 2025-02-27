Project Algorithmic Paper Trading with Java
Author: Jason Lee 2/26/2025
Revision history:


Executive Summary:

To create a paper trading platform that can test out user's ideas with the use of Java, Springboot and multithreading concepts

Introduction/Motivation:

With my other ML projects and personal theories for algorithmic trading, this project will try to emulate how a bank may paper trade test out algorithms for trading

Requirements:

  Functional Requirements:
    Market Data Ingestion
      Fetch live market data from API
      Process multiple dta feeds concurrently
    Trading strategy engine
      Evaluate market data 
      Implement various strategies
    Order Execution
    Dashboard
      Display results

  Non-functional Requirements
    Speed/low latency
    Scalability
    Security
    User friendliness

High-Level Design
    Market Data Ingestion 
    Trading Strategy Engine
    Order execution
    Dashboard

Detailed Design
   Market Data Ingestion Module
     PURPOSE:
       Fetch Data from various sources
     Design considerations:
       Utilize Spring
       Utilize ExecutorService
     Key components
       GET from polygon API

    Trading Strategy engine
      Evaluate marking data and apply strategy
       Use @Async

    Order execution
      Keep track of trades

    Dashboard
      Provide user a clear performance visualization

Dataflow
  Market Data -> Strategy selection -> Order execution and keep track -> Dashboard

Testing
  Unit testing with JUnit
  Integration Testing
  Optional:
    performance testing

Deployment
  Containerization
    Docker
  Ci/CD
    Jenkins

