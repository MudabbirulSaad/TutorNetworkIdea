# Product Requirements Document: TutorConnect

## 1. Introduction

TutorConnect is an innovative online tutoring platform that connects Australian students with skilled tutors from Bangladesh, primarily focusing on computer science and related subjects. The platform aims to provide affordable, high-quality tutoring while offering income opportunities for Bangladeshi students.

## 2. Product Overview

TutorConnect facilitates one-on-one tutoring sessions between Australian students and Bangladeshi tutors. The platform handles matching, scheduling, payment processing, and quality control, ensuring a seamless experience for both students and tutors.

## 3. Target Audience

- Primary: Australian university students struggling with specific unit topics, particularly in computer science
- Secondary: Skilled Bangladeshi students (primarily in computer science) looking for tutoring opportunities

## 4. Key Features

### 4.1 User Profiles
- Student profiles with academic information and tutoring needs
- Tutor profiles with expertise areas, ratings, and availability

### 4.2 Matching System
- Algorithm to match students with appropriate tutors based on subject, availability, and ratings

### 4.3 Scheduling System
- Calendar integration for easy session booking
- Time zone management between Australia and Bangladesh

### 4.4 Video Conferencing
- Built-in video call functionality with screen sharing
- Collaborative tools (e.g., whiteboard, code editor)

### 4.5 Recording Feature
- Option to record tutoring sessions
- Secure storage of recorded sessions
- Playback feature for students to review sessions

### 4.6 Payment System
- Secure international payment processing
- Tiered payment structure based on tutor ratings and experience

### 4.7 Rating and Review System
- Post-session rating and review submission for students
- Aggregate rating displayed on tutor profiles

### 4.8 Dispute Resolution
- System for students to claim refunds for unsatisfactory sessions
- Process for tutors to contest fraudulent claims
- Admin panel for reviewing disputes and recorded sessions

### 4.9 Tutor Incentive Program
- Perk system based on ratings and number of sessions conducted
- Higher pay rates for top-rated tutors

### 4.10 Payment Processing
- Integration with Stripe for receiving payments from Australian students
- Multiple payout options for Bangladeshi tutors:
  - Wise (formerly TransferWise)
  - Payoneer
  - Direct Bank Transfer (SWIFT)
  - Mobile Financial Services (bKash, Nagad)
- Real-time exchange rate calculations
- Tutor dashboard for earnings tracking and payout management

### 4.11 Commission Structure
- Percentage-based commission on each completed tutoring session
- Tiered commission rates based on tutor experience and ratings
- Transparent fee structure visible to both students and tutors

## 5. Technical Requirements

### 5.1 Platform
- Web-based application with responsive design
- Mobile apps for iOS and Android (future consideration)

### 5.2 Backend
- Scalable server architecture to handle concurrent video sessions
- Database to store user profiles, session data, and recordings
- API for frontend and potential future integrations

### 5.3 Frontend
- React-based web application
- User-friendly interface for both students and tutors

### 5.4 Video Conferencing
- Integration with a reliable WebRTC solution or third-party service

### 5.5 Payment System
- Integration with Stripe API for processing student payments
- Development of a custom payout system supporting multiple methods (Wise, Payoneer, Bank Transfer, MFS)
- Secure storage and handling of financial information
- Real-time currency conversion system

### 5.6 Data Storage and Security
- Secure, GDPR-compliant storage for user data and session recordings
- Encryption for all sensitive data

## 6. User Flow

1. Student signs up and creates a profile
2. Student searches for a tutor or requests a match
3. Student books a session with a tutor
4. Both parties join the video call at the scheduled time
5. Tutoring session is conducted and optionally recorded
6. Student rates the tutor and provides feedback
7. Payment is processed through Stripe
8. Platform calculates commission and tutor's share
9. Tutor selects preferred payout method
10. Platform initiates payout to tutor based on the selected method

## 7. Payment Processing Flow

### 7.1 Student Payment
1. Student initiates payment for a tutoring session
2. Stripe processes the payment in AUD
3. Funds are held in TutorConnect's Australian business account

### 7.2 Commission Calculation
1. Platform calculates the commission based on the session rate and tutor's tier
2. Remaining amount is allocated as tutor's earnings

### 7.3 Tutor Payout
1. Tutor selects preferred payout method (Wise, Payoneer, Bank Transfer, or MFS)
2. Platform initiates transfer based on selected method
3. Funds are converted from AUD to BDT using real-time exchange rates
4. Tutor receives payment in their Bangladeshi bank account or mobile wallet

### 7.4 Payout Methods
- Wise: Direct transfer to tutor's bank account
- Payoneer: Transfer to tutor's Payoneer account
- Direct Bank Transfer: SWIFT transfer to tutor's bank account
- Mobile Financial Services: Transfer to bKash or Nagad mobile wallet

## 8. Commission Structure

### 8.1 Base Commission
- Platform takes a 20% commission on each completed tutoring session

### 8.2 Tiered Commission Rates
- New tutors (0-50 hours): 20% commission
- Experienced tutors (51-200 hours): 18% commission
- Expert tutors (201+ hours): 15% commission

### 8.3 Performance Bonuses
- Tutors maintaining a 4.8+ rating over 20 sessions: Additional 2% reduction in commission

### 8.4 Transparency
- Commission rates and calculation method clearly displayed to tutors
- Students see all-inclusive pricing, with platform fees built into the displayed rate

## 9. Monetization

- Commission on each tutoring session as per the tiered structure
- Currency conversion fees (small percentage or fixed fee per transaction)
- Premium features for students (e.g., unlimited session recordings)
- Featured listings for tutors

## 10. Future Considerations

- Expansion to other subjects beyond computer science
- Integration with university learning management systems
- Group tutoring sessions
- AI-powered study tools and recommendations

## 11. Legal and Compliance

- Terms of Service and Privacy Policy
- Compliance with Australian and Bangladeshi labor laws
- Data protection in accordance with GDPR and local regulations
- Compliance with international money transfer regulations
- Clear terms of service regarding payment processing and commissions
- Data protection measures for financial information

## 12. Success Metrics

- Number of active users (students and tutors)
- Number of completed tutoring sessions
- Average student satisfaction rating
- Tutor retention rate
- Revenue growth
- Average commission per session
- Tutor satisfaction with payment process
- Percentage of successful payouts

## 13. Launch Plan

### Phase 1: MVP (Minimum Viable Product)
- Basic profile creation
- Matching system
- Video conferencing
- Payment processing (Stripe integration)
- Rating system

### Phase 2: Enhanced Features
- Session recording
- Dispute resolution system
- Tutor incentive program
- Multiple payout methods for tutors

### Phase 3: Scaling
- Mobile app development
- Expansion to additional subjects
- Integration with university systems
- Advanced analytics and reporting

## 14. Risks and Mitigation

| Risk | Mitigation Strategy |
|------|---------------------|
| Language barriers | Implement English proficiency requirements for tutors |
| Technical issues during sessions | Provide robust technical support and backup communication channels |
| Payment fraud | Implement secure payment gateways and fraud detection systems |
| Low-quality tutoring | Maintain strict quality control through ratings and dispute resolution |
| Timezone coordination | Develop an intuitive scheduling system with clear timezone indicators |
| Currency fluctuations | Implement real-time exchange rates and consider hedging strategies |
| Regulatory changes | Stay updated on international money transfer regulations and adapt quickly |
| Data security breaches | Implement strong encryption and regular security audits |

## 15. Conclusion

TutorConnect aims to revolutionize the online tutoring space by connecting Australian students with skilled Bangladeshi tutors. By focusing on computer science subjects initially, we can provide targeted, high-quality tutoring while offering valuable earning opportunities for Bangladeshi students. Our robust platform features, including advanced payment processing and a fair commission structure, will ensure a seamless experience for all users. As we progress through our launch phases, we will continuously refine our offering based on user feedback and market demands.
