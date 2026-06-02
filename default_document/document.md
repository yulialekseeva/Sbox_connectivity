# Message: BusinessMessageReject [j] (Market)

<div><div></div><div></div><div><table data-structure="Message Structure"><thead><tr><th colspan="3" align="center">BusinessMessageReject [j] (Market) - Message</th></tr><tr><th>Name</th><th>ID</th><th class="limitedMaxWidth">Description</th></tr></thead><tbody><tr><td style="width: 33%;"><div>&lt;StandardHeader&gt;<br>component</div></td><td style="width: 12%;"><div>1024</div></td><td style="width: 55%;"><div><div><div><div class="text">MsgType = j (lowercase)</div></div></div></div></td></tr><tr><td style="width: 33%;"><div>RefSeqNum</div></td><td style="width: 12%;"><div>45</div></td><td style="width: 55%;"><div><div><div><div class="text">MsgSeqNum of rejected message</div></div></div></div></td></tr><tr><td style="width: 33%;"><div>RefMsgType</div></td><td style="width: 12%;"><div>372</div></td><td style="width: 55%;"><div><div><div><div class="text">The MsgType of the FIX message being referenced.</div></div></div></div></td></tr><tr><td style="width: 33%;"><div>RefApplVerID</div></td><td style="width: 12%;"><div>1130</div></td><td style="width: 55%;"><div><div><div><div class="text">Recommended when rejecting an application message that does not explicitly provide ApplVerID ( 1128) on the message being rejected. In this case the value from the DefaultApplVerID(1137) or the default value specified in the NoMsgTypes repeating group on the logon message should be provided.</div></div></div></div></td></tr><tr><td style="width: 33%;"><div>BusinessRejectReason</div></td><td style="width: 12%;"><div>380</div></td><td style="width: 55%;"><div><div><div><div class="text">Code to identify reason for a Business Message Reject message.</div></div></div></div></td></tr><tr><td style="width: 33%;"><div>Text</div></td><td style="width: 12%;"><div>58</div></td><td style="width: 55%;"><div><div><div><div class="text">Where possible, message to explain reason for rejection</div></div></div></div></td></tr><tr><td style="width: 33%;"><div>&lt;StandardTrailer&gt;<br>component</div></td><td style="width: 12%;"><div>1025</div></td><td style="width: 55%;"></td></tr></tbody></table><br></div><div></div></div>
::BusinessMessageReject \[j\] (Market){#tbl:message_BusinessMessageReject_j_Market}


| Revision | Changes  | Details |
| --- | --- | --- | 
| 2.2.3.a | Removed: SecurityList (y, T-style); SecurityListUpdateReport (BK, T-style)|ForeignOwnershipRestriction (140) from InstrAttribType (871)|
|2.2.3 | Changed: SecurityList (y, T-style); SecurityListUpdateReport (BK, T-style) | Currency (15), StartDate (916), EndDate (917): More/Changed detail to field descriptions|
|2.2.3 |Added: SecurityList (y, T-style); SecurityListUpdateReport (BK, T-style)|ForeignOwnershipRestriction (140), MaxAllowedForeignOwnership (141) to InstrAttribType (871)|
|2.2.3 | Added: SecurityList (y, T-style); SecurityListUpdateReport (BK, T-style)| MaturityFrequencyUnit (2982), MaturityFrequencyPeriod (2983), CouponFrequencyUnit (1949), CouponFrequencyPeriod (1948), UnitOfMeasureCurrency (1716), FloatingRateIndexID (2731), FloatingRateIndexIDSource (2732), LegCouponType (2161), LegCouponFrequencyPeriod (2163), LegCouponFrequencyUnit (2164), LegCouponDayCount (2165), LegCurrency (556), NoLegEvents (2059), LegEventType (2060), LegEventTimeUnit (2063), LegEventTimePeriod (2064), LegBusinessDayConvention (40925), NoLegBusinessCenters (40923), LegBusinessCenter (40924), LegDateRollConvention (40926)| 
|2.2.2 | Changed: Appendices|Aligned Field Definition Changed and Field Definition Added (ET custom tag) with other FIX specifications|
|2.2.2 | Added: TradingSessionList (BJ)|SessionStateAdditionalInfo (29100)| 
|2.2.2 | Added: MarketDefinition (BU), SecurityList (x), SecurityListUpdateReport (BK)|MarketAdditionalInfo (29101), MarketSegmentAdditionalInfo (29102)|
|2.2.09.a | Changed (Errata): TradingSessionList (BJ) |tag name: SessionStateTypeNumber (28032)| 
|2.2.09.a | Cahanged (Errata): SecurutyList (y, out, 1465="T") |Cardinality = 1 .. 5 for NoSecurityClassifications (1582)| 
|2.2.09 |Added: Eqlipse Versions section||
|2.2.09 | Added: SecurityList, T-version | UnitOfMeasure (996), UnitOfMeasureQty (1147), UnitOfMeasureCurrency (1716) for nominal value|
|2.2.09 | Changed: About Req'd column section | Definition of values |
|2.2.09 | Changed: Req'd column: "Cond'l in ET" exchanged for "C" (conditional)| All occurences |
|2.2.09 |Added: About the Parties group section|PartyRole (452)  = Exchange (22)|
|2.2.09 |Added: SecurityListRequest (x)|Conditions when Symbol (55), MarketID (1301), MarketSegmentID (1300) apply and are required|
|2.2.09 |Added: SecurityListRequest (x)|Default value for SubscriptionRequestType (263) = Snapshot (0)|
|2.2.09 |Added: SecurityList (y), SecurityListUpdateReport (BK)  |AssetSubClassName (107), AssetSubClassID (108) to SecurityClassificationReason (1583)|
|2.2.09 |Changed (Errata): SecurityDefinition (BU)  |MarketSegmentDesc(1396) is optional|
|2.2.09|Changed: SecurityAltIDSource (456), UnderlyingSecurityIDSource (305),   LegSecurityAltIDSource (606)  |AssetID (127) (Changed from MMEAssetID|
|2.2.09|Added: About Price and Quantity|java long.minvalue|
|2.2.09|Added: SecurityList (y)|SecurityRejectReason (1607) to T, C, M variants|
|2.2.08|Added: BusinessMessageReject (j)|Explicit RefMsgType (372) values  |
|2.2.08| Added: MarketDefinition (BU)|PriceType (423)|
|2.2.07| Added: SecurityList (y, T-style), SecurityListUpdateReport (BK, T-style)|101 (Act/30) to PaymentStreamDayCount (40742)|
|2.2.07| Added: Chapter 1|Note on number of PartyRole and excess tags|
|2.2.07|Added: Section on FIX Version and Extension Packs||
| 2.2.07| Added (Errata): SecurityList (y), T-style; SecurityListUpdateReport (BK), T-style| SecurityStatus (965) = 9 (Suspended) |
|2.2.06| Added: SecurityList (y), T-style; SecurityListUpdateReport (BK), T-style| InstrAttribType (871) = 136 (NumberOfSettlementDays) |
| 2.2.06|Added: SecurityDefinitionRequest (c )|UnderlyingPx (810) |
|2.2.06|Changed: New layout of Spec|All content, Product rebranded to Eqlipse Trading|
|2.2.05| No changes| |
|2.2.04|Errata: SecurityDefinitionRequest (c )|871 = 11 only for SECLOAN|
|2.2.03|Added: Field Definitions Added|CorpAction custom component tags|
|2.2.03|Added: SecurityList (y), T-style; SecurityListUpdateReport (BK), T-style|SecurityClassificationReason (1583) = 105 (Listing board); SecurityClassificationValue (1584) = Listing board mnemonic|
|2.2.03|Added: SecurityList (y), C-style; SecurityListUpdateReport (BK), C-style|CorpActionExDate (29012); CorpActionPaymentDate (29013); CorpActionValue (29014)|
|2.2.03|Errata: TradingSessionList (BJ)|SessionStateTypeNumber (28032) explanation of use|
|2.2.03|Errata: SecurityList (y), M-style; SecurityListUpdateReport (BK), M-style|1465 = “M”|
|2.2.03|Errata: SecurityList (y), T-style; SecurityListUpdateReport (BK), T-style|PaymentStreamDayCount (40742) enumeration values|
|2.2.02|Corrected: SecurityListRequest (x)|SubscriptionRequestType (263) added back|
|2.2.01|Added: SecurityDefinitionRequest (c)|Symbol (55), SecurityI (48), SecurityIDSource (22), SecurityType (167), NoInstrAttrib (870) in AttrbGrp, InstrAttribType (871), InstrAttribValue (872), EndDate (917)|
|2.2.01|Added: SecurityDefinition (d)|SecurityRejectReason (1607): 105 = security Id invalid or not found|


***

|Revision|Changes  | Details |
| --- | --- | --- |
|2.2.3.a| Changed (Errata): TradingSessionSubID (625) | Datatype is String  |
|2.2.3.a|Added: TradeCaptureReport (AE, out, 1-side, matched|New matched confirmation as TradeCaptureReport of trade report matching|
| 2.2.3.a|Added: QuoteResponse (AJ, out)| Accepted (11) to QuoteResponseType (694) + Usage and Conditions entry|
| 2.2.3.a|Added: TradeCaptureReport (AE, out, 1-sided to cpty)|ExecType (150); TransBkdTime (483): Must match the counterparty side according to the configuration of the trade report type, only present when a valid timestamp was entered.. (clarification)|
| 2.2.3|Added: TradeCaptureReport (AE, in, 2-sided), TradeCaptureReport (AE, in, 1-sided), TradeCaptureReportAck (AR, out, 1-sided| SellShort (5) to Side (54)|
|2.2.3|Added: TradeCaptureReport (AE, in, 2-sided)|"IRS" to SecurityType (167); StartDate (916); Fixed income related description comments to 916, 64, 54 |
| 2.2.3|Added: TradeCaptureReportAck (AR, out, 2-sided)|IRS" to SecurityType (167); StartDate (916); EndDate (917); SettlDate (64)|
|2.2.2.a|Removed: NewOrderSingle (D), ExecutionReport (8), OrderCancelReplaceRequest (G) | Description text on default interpretation of TimeInForce = 0 as Day|
|2.2.2| Changed: OrderCancelReplaceRequest (G)|Limitations: Order with full quantity condition can be altered using either MinQty (110) or ExecInst (18)=G (+ more stringent wording)|
|2.2.2| Changed: Appendices|Aligned Field Definition Changed and Field Definition Added (ET custom tag) with other FIX specifications|
|2.2.2 | Removed: Appendices: 1-sided TCR matching flow| TradeCaptureReportAck (AR) will no longer convey a match to the initiating participant.|
|2.2.2| Added: TradeCaptureReport (AE, out, 1-sided) | Limitations: "It’s not possible to tell from the trade cancellation report whether it’s because of a withdrawal of the proposed trade from the initiator or because of a match."|
|2.2.2|Added: Quote (S) |Limitation (clarification): Only 1 quote per quote request per participant (not user)|
|2.2.2|Added: ExecRpt (8) |TrdRegTimestamps group|
| 2.2.2| Changed (Errata): OrderCancelReplaceRequest (G)|OrigClOrdID (41) is required |  
| 2.2.2| OrderCancelReplaceRequest (G)| TimeInForce (59): Field should be omitted if unchanged|
|2.2.2| Changed: ExecutionReport (8) |Usage and Conditions: OrdType (40=K (MarketWithLeftOverAsLimit) remark|
|2.2.2|Added: ExecutionReport (8)  |LastMkt (30), SecondaryExecID (527)|
|2.2.2|Added (Errata): OrderCancelRequest (F)|PartyRole (452) = 24 (CustomerAccount|
|2.2.2|Added: NewOrderSingle (D), ExecutionReport (8) |ExDestination (100): Only applicable to installations with order routing enabled|
|2.2.2|Removed: NewOrderSingle (D) |TradeDate (75)|
|2.2.14.b|Added: OrderCancelRequest (F)| Limitation: PartyRole=24 is accepted but not validated or returned|
|2.2.14.b|Changed: TradeCaptureReport (AE, in, 1-sided)| TradeHandlingInstr (1123) required also to cancel |
|2.2.14.b| Removed (Errata): TradeCaptureReport (AE, in, 2-sided)| SellShort (5) from Side (54)|
|2.2.14.b| Changed (Errata): QuoteRequest (R, in)| RespondentType (1172) is required|
|2.2.14.b| Changed (Errata): TradeCaptureReport (AE), ExecutionReport (8)| OrderID (37) has length [19]|
|2.2.14.b|Added: OrderCancelReplaceRequest (G) |Limitations: GTS order condition not available (clarification)|
|2.2.14.b| Removed: ExecutionReport (8)| EqlipseTradeType = 3, 5 (as only for reported trades) |
|2.2.14.b| Added: QuoteRequest (R), Quote (S), QuoteResponse (AJ)| Usage and Conditions: clarifying the RFQ Side convention in Eqlipse|
|2.2.14.b| Added: MassQuoteAck (b)| QuoteStatus (297) is set to Accepted if all quote entries could be passed on internally (clarification)|
|2.2.14.b| Removed (Errata): TradeCaptureReport (AE, out, 1-sided) | Limitations: "It’s not possible to tell from the trade cancellation report whether it’s because of a withdrawal of the proposed trade from the initiator or because of a match."|
|2.2.14.a| Changed (Errata): ExecutionReport (8) | Symbol (55) is required|
|2.2.14.a|Added: ExecutionReport (8)|Limitations: Remark on OrigClOrdID (41)|
|2.2.14.a|Removed: ExecutionReport (8)|4, 6, 36 for EqlipseTradeType (29076)|
|2.2.14.a|Added: OrderCancelRequest (F), ExecutionReport (8)|Usage and Conditions (F)/Limitations (8): Remark on mismatched Side values for cancellation|
|2.2.14|Added: Eqlipse Versions section||
|2.2.14|Changed: TradeCaptureReport (AE, out, 1-side, TradeCaptureReportAck (AR, 1-side + OnHold)|SecurityType (167) description: "Passthrough information"|
|2.2.14|Changed (Errata): ExecutionReport (8)|OrderID (37) = NONE for a rejected order|
|2.2.14|Added: ExecutionReport (8)|Limitations: For rejected order messages, instrument identifiers are echoed back as they were received (e.g. 48, 22 may be absent, Symbol (55) can be [N/A]) (no change)|
|2.2.14|Added: TradeCaptureReportAck (AR, out, 1-sided)|Limitations: For rejected trade reports, instrument identifiers are echoed back as they were received (e.g. 48, 22 may be absent); Symbol (55) can be [N/A] |
|2.2.14|Changed: NewOrderSingle (D), ExecutionReport (8)|TriggeringInstruction: all tags are now conditional and their individual presence conditions stated.|
|2.2.14|Added: ExecutionReport (8)|TradeTypeGrp, EqlipseTradeSubType (29076) for Deal Source|
|2.2.14| Removed: TradeCaptureReport (AE), TradeCaptureReportAck (AR)| SecurityType (167) = OTHER |
|2.2.14| Changed: Req'd column: "Cond'l in ET" exchanged for "C" (conditional)| All occurences |
|2.2.14|Added: About the Parties group section|PartyRole (452)  = Exchange (22)|
|2.2.14| Changed: About Req'd column section | Definition of values |
|2.2.14 | Added: ExecutionReport (8) |AggressorIndicator (1057)|
|2.2.14 | Changed: MassQuote (i) |BidPx (132), OfferPx (133) must be omitted for cancellation|
|2.2.14|Added: NewOrderSingle (D), ExecutionReport (8)|TriggerSecurityID (1104), TriggerSecurityIDSource (1105)|
|2.2.14|Added: About Price and Quantity|java long.minvalue|
|2.2.14| Added:  Added: Appendices |2-sided Trade Report flow|
|2.2.14| Added: ExecutionReport (8)| Parties group populates also for rejections, limitation removed|
|2.2.14| Removed: TradeCaptureReportAck (out, 2-side)| Cancelled (3) from TrdRptStatus (939)|
|2.2.14| Added: ExecutionReport (8)| SecurityID (48), SecurityIDSource (22)|
|2.2.13|Added: BusinessMessageReject (j)|Explicit RefMsgType (372) values  |
|2.2.13| Added: OrderCancelReplaceRequest (G)|Limitations: TimeInForce (59) must not be changed to FoK or IoC. |
|2.2.13| Removed (Errata): TradeCaptureReport (AE, in, 1-sided)|SellShort (5) from Side (54)|
|2.2.13| Changed: Flow diagrams|1-sided trade report flows for matched trades and cancel trade|
|2.2.13| Removed (Errata): TradeCaptureReportAck (out, on-hold)|PartyRole EnteringFirm (7), EnteringTrader (36)|
|2.2.13| Changed: TradeCaptureReport (in, 1-sided)|SecurityType (167) is required and validated|
|2.2.13| Added: Chapter 1|Note on number of PartyRole and excess tags|
|2.2.13|Added: Section on FIX Version and Extension Packs||
|2.2.13|Removed: TradeCaptureReport (AE, in, 1-sided)| TradeID (1003)|
|2.2.13|Changed (Errata): TradeCaptureReport (AE, in, 1-sided)| TradeHandlingInstr (1123) not needed to cancel |
|2.2.13 | Added (Errata): ExecutionReport (8)|Limitation: SecurityID (48), SecurityIDSource (22) not included |
|2.2.13 | Added: TradeCaptureReportAck (AR, out, 1-sided)|0 (New), H (TradeCancel) to ExecType (150), Limitation: No ExecType for rejected trade reports.|
|2.2.12 | Added (Errata): OrderCancelRequest (F, in), OrderCancelReplaceRequest (G, in) |SecurityID (48), SecurityIDSource (22)|
|2.2.12 | Added: SecurityDefinitionRequest (c, in), SecurityDefinition (d, out), BusinessMessageReject (j, out)  |support creation of Repos and TMC:s |
|2.2.12|Added: TradeCaptureReportAck (AR), out|Separate scenario for on-hold trades|
|2.2.12|Changed: TradeCaptureReportAck (AR), out, 2-sided  |Marked 167, 762, 573 as not req'd on rejection|
|2.2.12|Added: TradeCaptureReportAck (AR), out, 2-sided |F = Trade to ExecType (150)|
|2.2.12|Added: TradeCaptureReport (AE), in, 2-sided  |TransactTime (60) |
|2.2.12|Added: OrderCancelReplaceRequest (G), OrderCancelRequest (F), ExecutionReport (8), Section: How to update or cancel an order in different scenarios|PartyRole (452) = TraderMnemonic (53)|
|2.2.12|Added: NewOrderSingle (D), ExecutionReport (8)|ExDestination (100)|
|2.2.12|Changed: New layout of Spec|All content, FIX DC messages moved to separate spec. Product rebranded to Eqlipse Trading|
|2.2.11|Added: MassQuote (i), MassQuoteAck (b)|QuoteResponseLevel = 2 to QuoteResponseLevel (301), Affected entries in message properties table|
|2.2.11|Added: OneSidedAuctionRequest (UDD OneSidedAuctionRequestAck (UDE) OneSidedAuctionAction (UDF) OneSidedAuctionActionAck (UDG) OneSidedAuctionResult (UDH) |Messages for One-sided auction feature|
|2.2.11|Added: Added: NewOrderSingle (D),ExecutionReport (8)|Exec Instr (18) = 0, 6, 9 for Post only orders.|
|2.2.11|Changed: QuoteCancel (Z)|QuoteType (537) is required|
|2.2.10|Changed: ExecutionReport (8)|Limitations section: Parties group omitted when order rejected.|
|2.2.10|Added: NewOrderSingle (D) ExecutionReport (8)|MinQtyMethod (1822) Mention in limitations section for NOS, Mention in ExecInst (18) field description for NOS|
|2.2.10|Added: TradeCaptureReport (AE, in, 2-sided multileg) |SettlDate (64)|
|2.2.10|Added: MassQuote (i), MassQuoteAck (b |PartyRole (452), •  EnteringFirm (7), •  EnteringTrader (36)|
|2.2.10|Added: NewOrderSingle (D), ExecutionReport (8), OrderCancelReplaceRequest (G)|OrderRestrictions (529) = C (Issue Price Stabilization), Restructured Limitations section for OrderCancelReplaceRequest (G)|