# viyafruitgame
Game fruit
# classes.dex

.class public Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;
.super Ljava/lang/Object;
.source "FunEvent.kt"

# interfaces
.implements Lph/c;


# annotations
.annotation system Ldalvik/annotation/MemberClasses;
    value = {
        Lcom/kinkey/chatroom/repository/fun/proto/FunEvent$a;
    }
.end annotation


# static fields
.field public static final Companion:Lcom/kinkey/chatroom/repository/fun/proto/FunEvent$a;

.field public static final FUN_LUCKY_GIFT:I = 0x6

.field public static final FUN_PLACE_MESSAGE:I = 0x1

.field public static final FUN_TYPE_DICE_FUN:I = 0x4

.field public static final FUN_TYPE_DRAW_FUN:I = 0x3

.field public static final FUN_TYPE_FRUIT_GAME:I = 0x5

.field public static final FUN_TYPE_LUCKY_NUMBER:I = 0x1

.field public static final FUN_TYPE_LUCKY_WHEEL:I = 0x2

.field public static final FUN_TYPE_WEB_GAME:I = 0x64


# instance fields
.field private final funBody:Ljava/lang/String;

.field private funBodyObj:Lcom/kinkey/chatroom/repository/fun/proto/IFunBody;

.field private final funPlaceType:I

.field private final funType:I

.field private final specialRelationTheme:Lcom/kinkey/chatroom/repository/room/proto/SpecialRelationTheme;

.field private final userActiveMedals:Ljava/util/List;
    .annotation system Ldalvik/annotation/Signature;
        value = {
            "Ljava/util/List<",
            "Lcom/kinkey/appbase/repository/medal/proto/SimpleMedal;",
            ">;"
        }
    .end annotation
.end field

.field private final userActivePrivileges:Ljava/util/List;
    .annotation system Ldalvik/annotation/Signature;
        value = {
            "Ljava/util/List<",
            "Lcom/kinkey/appbase/repository/aristocracy/proto/UserPrivilege;",
            ">;"
        }
    .end annotation
.end field

.field private final userBroadcastUid:I

.field private final userChatTheme:Lcom/kinkey/chatroom/repository/room/proto/ChatTheme;

.field private final userFace:Ljava/lang/String;

.field private final userId:J

.field private final userLevel:Ljava/lang/Integer;

.field private final userName:Ljava/lang/String;

.field private final userWealthLevel:Ljava/lang/Integer;


# direct methods
.method public static constructor <clinit>()V
    .registers 1

    new-instance v0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent$a;

    invoke-direct {v0}, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent$a;-><init>()V

    sput-object v0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->Companion:Lcom/kinkey/chatroom/repository/fun/proto/FunEvent$a;

    return-void
.end method

.method public constructor <init>(JLjava/lang/String;Ljava/lang/String;IIILjava/lang/String;Ljava/lang/Integer;Ljava/lang/Integer;Ljava/util/List;Ljava/util/List;Lcom/kinkey/chatroom/repository/room/proto/ChatTheme;Lcom/kinkey/chatroom/repository/room/proto/SpecialRelationTheme;)V
    .registers 16
    .annotation system Ldalvik/annotation/Signature;
        value = {
            "(J",
            "Ljava/lang/String;",
            "Ljava/lang/String;",
            "III",
            "Ljava/lang/String;",
            "Ljava/lang/Integer;",
            "Ljava/lang/Integer;",
            "Ljava/util/List<",
            "Lcom/kinkey/appbase/repository/medal/proto/SimpleMedal;",
            ">;",
            "Ljava/util/List<",
            "Lcom/kinkey/appbase/repository/aristocracy/proto/UserPrivilege;",
            ">;",
            "Lcom/kinkey/chatroom/repository/room/proto/ChatTheme;",
            "Lcom/kinkey/chatroom/repository/room/proto/SpecialRelationTheme;",
            ")V"
        }
    .end annotation

    const-string v0, "userName"

    invoke-static {p3, v0}, Lut/j;->f(Ljava/lang/Object;Ljava/lang/String;)V

    const-string v0, "userFace"

    invoke-static {p4, v0}, Lut/j;->f(Ljava/lang/Object;Ljava/lang/String;)V

    const-string v0, "funBody"

    invoke-static {p8, v0}, Lut/j;->f(Ljava/lang/Object;Ljava/lang/String;)V

    .line 1
    invoke-direct {p0}, Ljava/lang/Object;-><init>()V

    iput-wide p1, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userId:J

    iput-object p3, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userName:Ljava/lang/String;

    iput-object p4, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userFace:Ljava/lang/String;

    .line 2
    iput p5, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userBroadcastUid:I

    iput p6, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->funType:I

    iput p7, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->funPlaceType:I

    .line 3
    iput-object p8, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->funBody:Ljava/lang/String;

    iput-object p9, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userLevel:Ljava/lang/Integer;

    iput-object p10, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userWealthLevel:Ljava/lang/Integer;

    .line 4
    iput-object p11, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userActiveMedals:Ljava/util/List;

    .line 5
    iput-object p12, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userActivePrivileges:Ljava/util/List;

    .line 6
    iput-object p13, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userChatTheme:Lcom/kinkey/chatroom/repository/room/proto/ChatTheme;

    .line 7
    iput-object p14, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->specialRelationTheme:Lcom/kinkey/chatroom/repository/room/proto/SpecialRelationTheme;

    return-void
.end method

.method public synthetic constructor <init>(JLjava/lang/String;Ljava/lang/String;IIILjava/lang/String;Ljava/lang/Integer;Ljava/lang/Integer;Ljava/util/List;Ljava/util/List;Lcom/kinkey/chatroom/repository/room/proto/ChatTheme;Lcom/kinkey/chatroom/repository/room/proto/SpecialRelationTheme;ILut/e;)V
    .registers 35

    move/from16 v0, p15

    and-int/lit16 v1, v0, 0x80

    const/4 v2, 0x0

    if-eqz v1, :cond_9

    move-object v12, v2

    goto :goto_b

    :cond_9
    move-object/from16 v12, p9

    :goto_b
    and-int/lit16 v1, v0, 0x100

    if-eqz v1, :cond_11

    move-object v13, v2

    goto :goto_13

    :cond_11
    move-object/from16 v13, p10

    :goto_13
    and-int/lit16 v0, v0, 0x400

    if-eqz v0, :cond_19

    move-object v15, v2

    goto :goto_1b

    :cond_19
    move-object/from16 v15, p12

    :goto_1b
    move-object/from16 v3, p0

    move-wide/from16 v4, p1

    move-object/from16 v6, p3

    move-object/from16 v7, p4

    move/from16 v8, p5

    move/from16 v9, p6

    move/from16 v10, p7

    move-object/from16 v11, p8

    move-object/from16 v14, p11

    move-object/from16 v16, p13

    move-object/from16 v17, p14

    .line 8
    invoke-direct/range {v3 .. v17}, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;-><init>(JLjava/lang/String;Ljava/lang/String;IIILjava/lang/String;Ljava/lang/Integer;Ljava/lang/Integer;Ljava/util/List;Ljava/util/List;Lcom/kinkey/chatroom/repository/room/proto/ChatTheme;Lcom/kinkey/chatroom/repository/room/proto/SpecialRelationTheme;)V

    return-void
.end method


# virtual methods
.method public final getFunBody()Ljava/lang/String;
    .registers 2

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->funBody:Ljava/lang/String;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getFunBodyObj()Lcom/kinkey/chatroom/repository/fun/proto/IFunBody;
    .registers 2

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->funBodyObj:Lcom/kinkey/chatroom/repository/fun/proto/IFunBody;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getFunPlaceType()I
    .registers 2

    .line 1
    iget v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->funPlaceType:I

    .line 2
    .line 3
    return v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getFunType()I
    .registers 2

    .line 1
    iget v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->funType:I

    .line 2
    .line 3
    return v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getSpecialRelationTheme()Lcom/kinkey/chatroom/repository/room/proto/SpecialRelationTheme;
    .registers 2

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->specialRelationTheme:Lcom/kinkey/chatroom/repository/room/proto/SpecialRelationTheme;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getUserActiveMedals()Ljava/util/List;
    .registers 2
    .annotation system Ldalvik/annotation/Signature;
        value = {
            "()",
            "Ljava/util/List<",
            "Lcom/kinkey/appbase/repository/medal/proto/SimpleMedal;",
            ">;"
        }
    .end annotation

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userActiveMedals:Ljava/util/List;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getUserActivePrivileges()Ljava/util/List;
    .registers 2
    .annotation system Ldalvik/annotation/Signature;
        value = {
            "()",
            "Ljava/util/List<",
            "Lcom/kinkey/appbase/repository/aristocracy/proto/UserPrivilege;",
            ">;"
        }
    .end annotation

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userActivePrivileges:Ljava/util/List;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getUserBroadcastUid()I
    .registers 2

    .line 1
    iget v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userBroadcastUid:I

    .line 2
    .line 3
    return v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getUserChatTheme()Lcom/kinkey/chatroom/repository/room/proto/ChatTheme;
    .registers 2

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userChatTheme:Lcom/kinkey/chatroom/repository/room/proto/ChatTheme;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getUserFace()Ljava/lang/String;
    .registers 2

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userFace:Ljava/lang/String;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getUserId()J
    .registers 3

    .line 1
    iget-wide v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userId:J

    .line 2
    .line 3
    return-wide v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getUserLevel()Ljava/lang/Integer;
    .registers 2

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userLevel:Ljava/lang/Integer;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getUserName()Ljava/lang/String;
    .registers 2

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userName:Ljava/lang/String;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final getUserWealthLevel()Ljava/lang/Integer;
    .registers 2

    .line 1
    iget-object v0, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->userWealthLevel:Ljava/lang/Integer;

    .line 2
    .line 3
    return-object v0
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
.end method

.method public final setFunBodyObj(Lcom/kinkey/chatroom/repository/fun/proto/IFunBody;)V
    .registers 2

    .line 1
    iput-object p1, p0, Lcom/kinkey/chatroom/repository/fun/proto/FunEvent;->funBodyObj:Lcom/kinkey/chatroom/repository/fun/proto/IFunBody;

    .line 2
    .line 3
    return-void
    .line 4
    .line 5
    .line 6
    .line 7
    .line 8
    .line 9
    .line 10
    .line 11
    .line 12
    .line 13
    .line 14
    .line 15
    .line 16
    .line 17
    .line 18
    .line 19
    .line 20
    .line 21
    .line 22
    .line 23
    .line 24
    .line 25
    .line 26
    .line 27
    .line 28
.end method
