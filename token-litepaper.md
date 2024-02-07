# OMA3 Token Litepaper

## 1. Executive Summary

OMA3 is a Web3 industry alliance, structured as a consortium, with the goal of ensuring an interoperable and user-owned metaverse. The consortium structure is one of the most proven mechanisms to enable industry collaboration, but consortia are only as good as the quality of member contributions.  Encouraging, tracking, and rewarding member contributions has always been a challenge in any industry collaboration and consortia are no different.  To solve this challenge, OMA3 is incorporating DAO elements into its governance.  This paper is our first step to creating a more effective collaboration structure for Web3.

Over the past few years Web3 projects have experimented using tokens to reward contribution or track reputation, expanding the utility of tokens beyond the more well-known use cases such as store of value and monetary transactions.  OMA3’s token architecture builds on such projects to enhance the usefulness of tokens in the context of collaboration.

The main purpose of the OMA3 token architecture is to track the reputation and contributions of consortium members.  The primary component of the architecture is a “soul-bound” non-fungible token (SBT).  An SBT is a non-fungible token (NFT) that cannot be transferred.  One SBT is allocated to each member and is included as part of membership.  The SBT stores the member’s OMA3 reputation. These SBTs are also used for tracking votes, as consortia overwhelmingly use a “one member/one vote” form of governance. This is in contrast to many Web3 DAOs which use “one fungible token/one vote” governance.

The second component of the OMA3 token architecture is the fungible token (FT).  In a previous version of this paper we mentioned that OMA3 has no plans for a fungible token.  This is no longer the case, and further development of both the OMA3 SBT and the FT will happen within OMA3’s working groups.

Reputation is the most important metric in OMA3’s token architecture and reputation points can be earned by contributing to OMA3 in various ways.  Reputation can also be lost under certain circumstances.  Reputation determines the privileges each member is granted by OMA3, including co-marketing, recognition, FT allocations, and any other benefit OMA3 may decide to bestow in the future.  One of the biggest drivers of reputation is OMA3’s bounty system.  Members can use the OMA3 bounty system to propose work that needs to be accomplished by OMA3, and members can apply to do the work described by the bounty.  Bounty award decisions are made initially by OMA3 leadership based on applicable member contributions. Over time bounty award decisions will be made through a more decentralized process such as public bounty proposals.

The purpose of this paper is to lay the foundation for OMA3’s token architecture, and be a starting point for the remaining work that will be accomplished in OMA3’s Token Working Group (TWG).
## 2. Background

### 2.1 OMA3

OMA3 is an industry alliance structured as a Swiss association.  The goal of OMA3 is to create specifications, software repositories, and infrastructure that enable the interoperable, user-owned metaverse.  

OMA3 is governed like a typical modern industry consortium.  Details on this governance framework are located in the [OMA3 Organizational Documents](https://assets.website-files.com/62a88c8ec868deb8bcfa3353/63611fb302b730108a90e482_oma3-complete-signable.pdf).  To summarize, OMA3 has three tiers of member participation:

  * Community Member:  This is the most accessible membership level with benefits that include invitations to the OMA3 Discord channel, membership SBTs, possible participation in future airdrops, and rights to review and comment on OMA3 work products before they become final.  OMA3 has yet to activate this membership level as of January 2024.

  * Creator Member:  Creator Members receive all the rights of Community Members, plus participation and voting rights in OMA3 working groups as well as the right to be nominated to OMA3 leadership positions such as working group chairs.  This membership level is open to any organization.

  * Sponsor Member:  Sponsor Members receive all the rights of Creator Members, plus the right to nominate one individual to the OMA3 Board of Directors as a voting member.  Sponsor Members are elected by the OMA3 Board and reputation plays a large role in this election.

Consortia are responsible for creating some of the most widely used technologies in the world, but there is a “tragedy of the commons” in consortia wherein members are incentivized to let others do the work of running working groups, creating specifications, and writing code because all members benefit the same regardless of whether they do the work or not.	OMA3 intends to change these incentives by rewarding members based on their contributions, thereby encouraging members to do the necessary work.

### 2.2 Stakeholders

There are many types of stakeholders that play a role in the OMA3 token architecture.  OMA3 members (Sponsor Members, Creator Members, and Community Members) play the biggest role as each SBT is tied to a member.  The other big roles are filled by OMA3 leaders, employees, service providers, implementers, and users.

#### 2.2.1 Leaders

OMA3 leaders are individuals who have added OMA3 governance responsibility beyond the responsibilities of other member representatives.  Leaders include OMA3 officers (Chairperson, Secretary, Treasurer, Vice Chairs, and other roles held by OMA3 representatives), working group leaders (chairs, vice-chairs, project managers, and open source maintainers that are members of OMA3), and committee leaders (Sponsor Member representatives that run board-level committees).  Current leaders can be found at OMA3.org.

#### 2.2.2 Employees

OMA3 employees include staff directly hired by OMA3 such as CTO, CMO, and operations director.  These positions can be occupied by member representatives or be individuals employed directly by OMA3.

#### 2.2.3 Service Providers

OMA3 members can provide services to OMA3, and if these services are provided at a discount these discounts can be tracked in the member’s SBT.  Service providers include consultants, contractors, accounting firms, marketing and PR firms, attorneys, and event planners.

#### 2.2.4 Implementers

Implementers include any organization that uses the work product of OMA3 to build and/or offer products and services, including developers, exchanges, and wallet providers.  Implementers can be members or non-members, but only member implementers receive benefits from OMA3.

#### 2.2.5 Users

Users are individuals who are not OMA3 members, yet still use products or services that incorporate OMA3 work products.  In the future, individuals will also be able to join OMA3 as members.

## 3. Soulbound Membership NFT

### 3.1 SBT Structure

Each OMA3 member receives an SBT that is non transferable.  Which chain(s) OMA3 SBTs reside on will be determined in the future.  

To protect OMA3 operations, SBTs are controlled by wallets sanctioned by OMA3.  OMA3 enforces security and access control requirements for SBT wallets.  Access control requirements may be different depending on the level of membership.  Each SBT wallet must be stored on an OMA3-approved multi-sig wallet which requires at least two signers for every transaction signature.  Individual multisig signers must also use an OMA3-approved wallet. The complete list of such wallets will be composed and published in the future.  An organization may only transfer control of its wallet to affiliate organizations.

KYC checks will be used for all corporate and individual signers.  Details on KYC will be worked out in the TWG.

The OMA3 SBT is compliant with the W3C Decentralized Identifiers (DID) specification:

  * DID Verifiable Credential (“VC”)- The DID VC is the software object that is the actual identity credential.  In the OMA3 token architecture, the VC is the OMA3 SBT.
  * DID Holder- A Holder in the W3C specification is the entity that is represented by the VC.  In the OMA3 SBT model, the DID Holder is the OMA3 member
  * DID Issuer- An Issuer in the W3C specification is the entity that gives out the VC and vouches for the authenticity of the VC by signing it.  With OMA3 SBTs, OMA3 is the Issuer.

The  privacy-preserving characteristic of DIDs could be useful as OMA3 explores privacy requirements for the SBT.  Currently there are no existing Verifiers besides OMA3, although this is expected to change as OMA3 grows.

### 3.2 SBT Functionality

An OMA3 SBT stores the following data (see Figure 1):

  * Identity
    * Member name and unique ID
    * Current official representatives
    * Affiliates that are also OMA3 members (if any)
  * Membership
    * Changes in membership status, including the new membership level (Sponsor, Creator, Community, or Non-Member) and the time of status change
    * Membership fees paid and date of payment
  * Participation records
    * Meeting attendance (Working groups, committees, General Assembly, Board of Directors)
    * Representing OMA3 at events
    * Voting records
  * Contributions
    * Contributions within the OMA3 Bounty System (see below)
    * Monetary contributions beyond membership fees
    * Time spent by OMA3 Leaders (see Stakeholders above) on OMA3
    * Fee discounts on services (e.g.- providing web development services)
    * Official comments on draft working product (e.g.- comments on specifications)
    * Other contributions approved by OMA3 that have monetary value
  * Adoption Metrics (TBD based on working group recommendations), for example:
    * Gas fees paid using an OMA3 smart contract
    * User referrals
    * Fees for using OMA3 infrastructure

### 3.3 Privacy

Members may not want some of the data stored in SBTs to be available to the public.  Members may not even want the data to be available to other members.  The Token Working Group will specify the correct privacy preserving mechanisms based on the nature of the data and the level or privacy needed.

![Figure 1]()
**Figure 1- SBT mechanics**

## 4. OMA3 Fungible Token

The OMA3 Fungible Token (FT) complements the SBT in OMA3’s token architecture.  However, whereas the SBT is strictly used for internal OMA3 operations, the FT is used for both internal operations and public OMA3 infrastructure.

### 4.1- Utility

Although FTs will not be used for voting (that is handled by SBTs), they will still have an integral role in OMA3 operations such as staking for board reputation or depositing collateral for fulfilling a bounty (see Section 7.2).  OMA3 working groups also have the option to integrate the FT into the infrastructure they provide.  For example, the Portaling and Mapping Working Group (PMWG) released a [Request for Proposals](https://github.com/oma3dao/iwps-rfp) (RFP) for the Inter World Portaling System (IWPS).  Section 12 of the RFP describes an optional requirement of staking and paying teleportation fees (“gas-like” fees) in IWPS.  The FT could be one of the tokens used for these features.

### 4.2- Allocation

The FT will be distributed in phases with the total supply divided into the following categories:

  * OMA3 Warchest (25%)
	* Treasury
	* Additional Liquidity
	* Reserves
  * Initial Liquidity (5%)
	* To support market making activities for AMMs.
  * Founders (5%)
  	* Founding members of OMA3 are given an allocation of tokens for creating OMA3.
    	* Founding members include:
   		* Animoca Brands
  	 	* Dacoco
   		* MultiversalME
  	 	* Space
   		* Superworld
  	 	* The Sandbox
   		* Upland
  * Investor Allocation (10%)
	* OMA3 can sell up to 10% of total supply to early token buyers.
    	* Funds from early token sales could allow OMA3 to lower membership fees, thereby diversifying its membership, and fund infrastructure development.
  * Ecosystem Rewards (55%)
* Contributions (Section 5)
   		* Member contributions to OMA3 are tracked using a reputation point system.
  	 	* FTs are allocated pro-rata based on points.
* Adoption (Section 6)
	* OMA3 will create verifiable metrics to track a member’s impact on adoption of OMA3 infrastructure.
		* FTs will be allocated based on these adoption metrics.

## 5. Contributions

Member companies contribute to OMA3, in working groups and outside of working groups.  These contributions are recorded in member SBTs and centralized data stores.  This data is used to calculate the aforementioned reputation points of a member.  Reputation points are calculated in an objective manner, based on multiple transparent mechanisms.

### 5.1- Contribution mechanics

Meeting attendance is one of the ways members can accrue reputation points.  Members that attend more meetings accrue more reputation points than members that do not.  As OMA3 grows the exact mechanism may change to discourage point farming.

OMA3 members can also accrue points by allowing their representatives to hold leadership roles.  Representatives can also provide a valuable service, such as financial accounting.  These contributions can be tracked in terms of points per hour:

* Officer/Working group chair compensation
	* Officers and working group leaders accrue points for contributing time to OMA3.
	* Time spent in working group meetings and Board meetings are not double-counted with attendance rewards.

* Service provider compensation
	* Service providers can accrue reputation for providing service at a reduced rate.
	* Service providers that accrue reputation must become a member of OMA3 (any membership tier).

### 5.2- Bounties

Bounties are a special mechanism for members to earn reputation and privileges by contributing to OMA3.  There are two types of bounties:  bounties governed by the Board (“Board Bounties”) and bounties governed by the Board and Working Groups (“Working Group Bounties”) (see Figure 2).  There are two ways to earn reputation with bounties:

* Create a Board Bounty:  Submit a proposal to create a bounty for fulfilling a board-level need such as creating a working group or a creating topic for a working group to address.  Members that submit Board Bounty creation proposal(s) that end up getting approved by the Board will receive a reputation reward. The reward for submitting a Board Bounty creation proposal is the same for each bounty creation proposal.  If proposals are very similar, only one will be approved.  Bounty proposers may recommend a reward for members that fulfill the bounty, but proposals to fulfill the bounty can set their own reward which may be different from the recommended reward.  Creating Working Group Bounties do not earn rewards because they are proposed by the working group chairs, and chairs already earn reputation points for leading working groups

* Fulfill a bounty (Board or Working Group):  For any open bounty, a member may submit a fulfillment proposal (e.g.- nominate for a leadership or individual contributor role, submit a document, write code, etc.).  The fulfillment proposal may indicate acceptance of a bounty fulfillment review process (see below). If conditions permit, the Board or working group may approve multiple fulfillment proposals for a bounty.


Board Bounties are initially awarded by the Board.  The Board takes into account the following factors when rewarding a bounty:
	* Capability of the member submitting the fulfillment proposal
* The nature of the work for the bounty (e.g.- creating a specification)
* Proposed reward for fulfilling the bounty
* Reputation of the members submitting the fulfillment proposal, as stored in SBTs and other storage mechanisms
* Collateral (“stake”) put up by the fulfillment proposers that can be lost if the proposers are unable to deliver.

Working Group Bounties are decided by a vote in working groups, but the vote must also be ratified by the Board.

OMA3 currently implements bounties for the following actions:

* Press placements- OMA3 rewards members that get OMA3 in the news, whether it be online publications or podcasts.
* New member referrals- OMA3 rewards members that recruit a company into becoming an OMA3 member.
* Specification contributions- OMA3 rewards members that contribute to specification documents and other tasks that are required for the creation and success of standards and related infrastructure.

Some bounty rewards pay out over time, not all at once.  For example, a large software project may pay rewards on alpha, beta, and production milestones.  Infrastructure may require a long period of production use before final rewards get paid out.  The payout schedule is up to the bounty.  For example, 50% of a bounty reward may be paid out on project completion and 50% may be held back pending a review of project performance.

![Figure 2]()
**Figure 2- Bounty system diagram**


## 6. Adoption Rewards

The success of OMA3’s projects depends on adoption as well as implementation.  To encourage adoption OMA3 will set aside an allocation of FTs to distribute to members based on adoption metrics.  For example, IWPS could award reputation points based on the number of teleportations originating from a member’s platform.  The NFT Working Group could track the total value of royalties paid by marketplaces to creators that use OMA3’s royalty system.  By rewarding both infrastructure developers and adopters OMA3 ensures the proper incentives are in place for OMA3 to accomplish its mission.  The specifics of the adoption reward mechanism will be developed in the OMA3 Technical Working Group.

## 7. Token Rollout

There are three phases to OMA3’s fungible token (FT) rollout.  Phase 1 is focused on architecture and initial implementation.  Phase 2 focuses on internal use and starts when the FT is first distributed to OMA3 members.  Phase 3 begins when the FT is first sold outside OMA3 membership.

### 7.1- Phase 1:  Pre launch

In Phase 1 there is no fungible token and contributions are recorded as reputation points in centralized data stores.  The goal of Phase 1 is to implement the token system that will be used in OMA3 operations, and deliver the roadmap for how the FT will be used in OMA3 infrastructure.  When OMA3 first distributes the FT, the FT will be distributed to members based on reputation points in the centralized data stores, at which point Phase 2 starts.

### 7.2- Phase 2:  Internal use

Once OMA3 token infrastructure is functional and Phase 1 FTs are distributed, OMA3 enters Phase 2 of the token rollout. In Phase 2 functionality of SBTs and FTs are limited to internal OMA3 operations and FTs cannot be transferred outside of OMA3 membership (see the OMA3 [Token Working Group MVP RFP](https://github.com/oma3dao/token-mvp-rfp) for details).  The Phase 2 feature set includes:

* SBTs store membership status
* SBTs track a member’s representatives
* SBTs track meeting attendance
* Bounty creation
* Bounty tracking in SBTs
* Tracking leadership positions in SBTs
* Staking FTs for access to different membership levels
* Staking FTs for bounty proposals
* Member-to-member FT transfers.

In Phase 2 OMA3 also begins to expand the community by offering new membership tiers, including:

* The Community Member tier for organizations
* Individual membership tiers that allow individuals to participate in the OMA3 community.

Membership fees will either be non-existent or very low, so cost will not be a deterrent for anyone.  These new membership tiers will have fewer governance rights when compared to Sponsor and Creator Members, but becoming a Creator Member will always be an option.

Since FTs are airdropped to members rather than being sold to members there is no VAT implication.  However, OMA3 may require recipients of initial FT distributions to hold FTs for a certain period of time before transferring them to entities that are not OMA3 members, or receiving monetary value for the FTs.

### 7.3- Phase 3: Public launch

OMA3 enters Phase 3 of the rollout when the following criteria are met:

* OMA3 membership grows to hundreds or thousands of active members.
* OMA3 infrastructure is functional and is able to utilize FTs.
OMA3’s public infrastructure will be used by non-OMA3 members, and if the infrastructure requires FTs then the FTs will need to be made available to non-members.  There are multiple ways do to this, including:

* OMA3 member platforms transferring FTs to their users inside their platforms.
* OMA3 member platforms abstracting FTs away from users by holding and transacting FTs on behalf of users.
* OMA3 members making FTs available for purchase on decentralized exchanges.
* OMA3 working with centralized exchanges to sell FTs.

In Phase 3, tokens are earned as follows:

* Adoption
	* Tokens are allocated to members that increase adoption of OMA3 technology.
	* All members (see caveats in Section 8 below) are eligible for this benefit.
	* This allocation is based on a TBD confirmable metric.
* Phase 3 Contributions
	* Since the fungible token has a market price in Phase 3 (at least after the initial holding period), all contributions (bounties, compensation, investments) will be paid in tokens out of this allocation.
* Tokens in the OMA3 Warchest can be re-allocated to Phase 3 tokens if necessary.


### 7.4- No Action

OMA3 will take no action to facilitate trading of OMA3 FTs in jurisdictions where it may be contrary to law.  OMA3 will require its members to take the same no action as well.


## 8. Legal Considerations

OMA3 is fully aware of the regulatory environment and recent enforcement actions against several Web3 projects.  Design and implementation of this OMA3 token architecture may need to change based on the resolution of these actions or guidance given by regulatory agencies and legislative bodies.  

Certain regulatory environments, such as the United States, China, and Russia, may restrict access to the FT.  If necessary, OMA3 will exclude certain entities from holding the FT.  Since the FT is expected to have utility in OMA3 infrastructure (to be decided by the TWG), OMA3 will allow entities in these countries to participate in OMA3 infrastructure in ways that do not require holding the FT, such as providing abstraction technology that allows participants to use OMA3 infrastructure without holding the FT. Neither holders of SBTs nor others have a legal claim to FTs and the issuance of FTs is at the sole discretion of OMA3.

OMA3 believes in the value this token architecture brings to both OMA3 and the Web3 metaverse as a whole.  We are committed to realizing this value in a regulatory compliant manner.

## Authors

### Mohamed Ezeldin
**[Animoca Brands](https://www.animocabrands.com)**, Head of Tokenomics   
**OMA3**, Token Working Group Chair


### Jerry Lai
**[Animoca Brands](https://www.animocabrands.com)**, Tokenonics Analyst   
**OMA3**, Token Working Group Vice Chair


### Alfred Tom
**[Wivity](https://www.wivity.com)**, CEO  
**OMA3**, Executive Director

## Public Comments
Create an issue on Github:  [https://github.com/oma3dao/public-documentation/](https://github.com/oma3dao/public-documentation/)   
Comment in [Google Docs](https://docs.google.com/document/d/1Yy2gHu2O3PfeatVwIpcu_j5XKSEttLvjG7LCnq6Cjwc/edit?usp=sharing)

## Get Involved
Become a member:  [https://www.oma3.org/join](https://www.oma3.org/join)

Joint the community: @oma3dao
[https://www.linkedin.com/company/oma3/](https://www.linkedin.com/company/oma3/)

## Stay Connected
Contact us:  info@oma3.org

Subscribe to our newsletter: [https://www.oma3.org/join-newsletter](https://www.oma3.org/join-newsletter)
